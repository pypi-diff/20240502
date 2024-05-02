# Comparing `tmp/inferio_x-0.1.0.tar.gz` & `tmp/inferio_x-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inferio_x-0.1.0.tar", max compression
+gzip compressed data, was "inferio_x-0.1.1.tar", max compression
```

## Comparing `inferio_x-0.1.0.tar` & `inferio_x-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1429 2023-12-07 15:01:13.995782 inferio_x-0.1.0/README.md
--rw-r--r--   0        0        0      237 2023-12-07 15:01:27.539839 inferio_x-0.1.0/inferio_x/__init__.py
--rw-r--r--   0        0        0      596 2023-12-07 14:48:36.425031 inferio_x-0.1.0/inferio_x/_background.py
--rw-r--r--   0        0        0      275 2023-12-07 14:47:45.592897 inferio_x-0.1.0/inferio_x/_configs.py
--rw-r--r--   0        0        0      497 2023-12-07 14:48:38.717038 inferio_x-0.1.0/inferio_x/_endpoint.py
--rw-r--r--   0        0        0     1339 2023-12-07 14:48:40.705043 inferio_x-0.1.0/inferio_x/_exceptions.py
--rw-r--r--   0        0        0      458 2023-12-07 14:47:45.592897 inferio_x-0.1.0/inferio_x/_file.py
--rw-r--r--   0        0        0      491 2023-12-07 14:47:45.592897 inferio_x-0.1.0/inferio_x/_log.py
--rw-r--r--   0        0        0       78 2023-12-07 14:47:45.592897 inferio_x-0.1.0/inferio_x/_method.py
--rw-r--r--   0        0        0      238 2023-12-07 14:47:45.592897 inferio_x-0.1.0/inferio_x/_response.py
--rw-r--r--   0        0        0     6378 2023-12-07 14:48:43.289050 inferio_x-0.1.0/inferio_x/_service.py
--rw-r--r--   0        0        0     1087 2023-12-07 14:48:45.093055 inferio_x-0.1.0/inferio_x/_utils.py
--rw-r--r--   0        0        0     1308 2023-12-07 15:01:20.947811 inferio_x-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2579 1970-01-01 00:00:00.000000 inferio_x-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1429 2024-05-02 06:23:11.353645 inferio_x-0.1.1/README.md
+-rw-r--r--   0        0        0      237 2024-05-02 08:23:40.103215 inferio_x-0.1.1/inferio_x/__init__.py
+-rw-r--r--   0        0        0      596 2024-05-02 06:23:11.354119 inferio_x-0.1.1/inferio_x/_background.py
+-rw-r--r--   0        0        0      341 2024-05-02 08:20:21.311688 inferio_x-0.1.1/inferio_x/_configs.py
+-rw-r--r--   0        0        0      497 2024-05-02 06:23:11.354426 inferio_x-0.1.1/inferio_x/_endpoint.py
+-rw-r--r--   0        0        0     1339 2024-05-02 06:23:11.354561 inferio_x-0.1.1/inferio_x/_exceptions.py
+-rw-r--r--   0        0        0      458 2024-05-02 06:23:11.354703 inferio_x-0.1.1/inferio_x/_file.py
+-rw-r--r--   0        0        0      491 2024-05-02 06:23:11.354835 inferio_x-0.1.1/inferio_x/_log.py
+-rw-r--r--   0        0        0       78 2024-05-02 06:23:11.354962 inferio_x-0.1.1/inferio_x/_method.py
+-rw-r--r--   0        0        0      238 2024-05-02 06:23:11.355102 inferio_x-0.1.1/inferio_x/_response.py
+-rw-r--r--   0        0        0     6448 2024-05-02 08:20:25.583526 inferio_x-0.1.1/inferio_x/_service.py
+-rw-r--r--   0        0        0     1087 2024-05-02 08:05:23.339828 inferio_x-0.1.1/inferio_x/_utils.py
+-rw-r--r--   0        0        0     1240 2024-05-02 08:23:31.735308 inferio_x-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2477 1970-01-01 00:00:00.000000 inferio_x-0.1.1/PKG-INFO
```

### Comparing `inferio_x-0.1.0/README.md` & `inferio_x-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `inferio_x-0.1.0/inferio_x/_background.py` & `inferio_x-0.1.1/inferio_x/_background.py`

 * *Files identical despite different names*

### Comparing `inferio_x-0.1.0/inferio_x/_exceptions.py` & `inferio_x-0.1.1/inferio_x/_exceptions.py`

 * *Files identical despite different names*

### Comparing `inferio_x-0.1.0/inferio_x/_service.py` & `inferio_x-0.1.1/inferio_x/_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from starlette.middleware import Middleware
 from starlette.middleware.cors import CORSMiddleware
 from starlette.requests import Request
 from starlette.status import HTTP_200_OK
 from starlette_exporter import PrometheusMiddleware, handle_metrics
 
 from inferio_x._background import send_log
-from inferio_x._configs import INFERIO_APP_NAME
+from inferio_x._configs import INFERIO_APP_NAME, TIMEOUT_KEEP_ALIVE
 from inferio_x._endpoint import Endpoint
 from inferio_x._exceptions import exception_handlers
 from inferio_x._file import FileUpload
 from inferio_x._log import Log, SuccessData
 from inferio_x._method import Method
 from inferio_x._response import OrJSONResponse
 
@@ -181,8 +181,9 @@
         uvicorn.run(
             self.app,
             host=self.host,
             port=self.port,
             access_log=self.access_log,
             log_level="info",
             use_colors=False,
+            timeout_keep_alive=TIMEOUT_KEEP_ALIVE
         )
```

### Comparing `inferio_x-0.1.0/inferio_x/_utils.py` & `inferio_x-0.1.1/inferio_x/_utils.py`

 * *Files identical despite different names*

### Comparing `inferio_x-0.1.0/pyproject.toml` & `inferio_x-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 [tool.poetry]
 name = "inferio-x"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Portmind's ML Engineering Team"]
 maintainers = [
     "Sevak Harutyunyan <sevak.harutyunyan@portmind.com>",
     "Tigran Vardanyan <tigran.vardanyan@portmind.com>",
     "Armen Gabrielyan <armen.gabrielyan@portmind.com>",
     "Vaghinak Vardanyan <vaghinak.vardanyan@portmind.com>"
 ]
 packages = [{include = "inferio_x"}]
 readme = "README.md"
-repository = "https://github.com/portmind/inferio"
+repository = "https://github.com/portmind/inferio-x"
 classifiers = [
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11'
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-uvicorn = "^0.24.0"
-starlette = "^0.32.0"
-httpx = "^0.25.2"
-uvloop = "^0.19.0"
-httptools = "^0.6.1"
-pydantic = "^2.5.2"
-orjson = "^3.9.10"
-starlette-exporter = "^0.17.1"
+uvicorn = "~0.29"
+starlette = "~0.37"
+httpx = "~0.27"
+pydantic = "~2.7"
+orjson = "~3.10"
+starlette-exporter = "~0.21"
 python-multipart = { version = "^0.0.5", optional = true }
 
 [tool.poetry.extras]
 fileupload = ["python-multipart"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pre-commit = "^3.5.0"
 commitizen = "^3.2.2"
-numpy = "^1.20.0"
 pytest-cov = "^3.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `inferio_x-0.1.0/PKG-INFO` & `inferio_x-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: inferio-x
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
-Home-page: https://github.com/portmind/inferio
+Home-page: https://github.com/portmind/inferio-x
 Author: Portmind's ML Engineering Team
 Maintainer: Sevak Harutyunyan
 Maintainer-email: sevak.harutyunyan@portmind.com
 Requires-Python: >=3.8,<4.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: fileupload
-Requires-Dist: httptools (>=0.6.1,<0.7.0)
-Requires-Dist: httpx (>=0.25.2,<0.26.0)
-Requires-Dist: orjson (>=3.9.10,<4.0.0)
-Requires-Dist: pydantic (>=2.5.2,<3.0.0)
+Requires-Dist: httpx (>=0.27,<0.28)
+Requires-Dist: orjson (>=3.10,<3.11)
+Requires-Dist: pydantic (>=2.7,<2.8)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6) ; extra == "fileupload"
-Requires-Dist: starlette (>=0.32.0,<0.33.0)
-Requires-Dist: starlette-exporter (>=0.17.1,<0.18.0)
-Requires-Dist: uvicorn (>=0.24.0,<0.25.0)
-Requires-Dist: uvloop (>=0.19.0,<0.20.0)
-Project-URL: Repository, https://github.com/portmind/inferio
+Requires-Dist: starlette (>=0.37,<0.38)
+Requires-Dist: starlette-exporter (>=0.21,<0.22)
+Requires-Dist: uvicorn (>=0.29,<0.30)
+Project-URL: Repository, https://github.com/portmind/inferio-x
 Description-Content-Type: text/markdown
 
 # InferIO-X
 
 Inference I/O Extended
 
 ![Python](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-brightgreen)
```

