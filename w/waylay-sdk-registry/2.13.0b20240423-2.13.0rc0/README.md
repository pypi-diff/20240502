# Comparing `tmp/waylay_sdk_registry-2.13.0b20240423.tar.gz` & `tmp/waylay-sdk-registry-2.13.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_registry-2.13.0b20240423.tar", last modified: Wed Apr 24 07:43:58 2024, max compression
+gzip compressed data, was "waylay-sdk-registry-2.13.0rc0.tar", last modified: Fri Mar 29 13:21:52 2024, max compression
```

## Comparing `waylay_sdk_registry-2.13.0b20240423.tar` & `waylay-sdk-registry-2.13.0rc0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:58.652392 waylay_sdk_registry-2.13.0b20240423/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-24 07:43:52.000000 waylay_sdk_registry-2.13.0b20240423/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-24 07:43:58.652392 waylay_sdk_registry-2.13.0b20240423/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-24 07:43:52.000000 waylay_sdk_registry-2.13.0b20240423/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-24 07:43:52.000000 waylay_sdk_registry-2.13.0b20240423/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 07:43:58.652392 waylay_sdk_registry-2.13.0b20240423/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:58.644392 waylay_sdk_registry-2.13.0b20240423/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:58.644392 waylay_sdk_registry-2.13.0b20240423/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:58.644392 waylay_sdk_registry-2.13.0b20240423/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:58.644392 waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:58.648392 waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/api/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-24 07:43:52.000000 waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-24 07:43:52.000000 waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/api/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    19352 2024-04-24 07:43:52.000000 waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   176732 2024-04-24 07:43:52.000000 waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/api/models_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   184941 2024-04-24 07:43:52.000000 waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/api/plugs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:52.000000 waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    44693 2024-04-24 07:43:52.000000 waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/api/runtimes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13348 2024-04-24 07:43:52.000000 waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/api/schemas_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   177971 2024-04-24 07:43:52.000000 waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/api/webscripts_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:58.648392 waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/service/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-24 07:43:52.000000 waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:52.000000 waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/service/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-24 07:43:52.000000 waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:58.652392 waylay_sdk_registry-2.13.0b20240423/src/waylay_sdk_registry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-24 07:43:58.000000 waylay_sdk_registry-2.13.0b20240423/src/waylay_sdk_registry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-24 07:43:58.000000 waylay_sdk_registry-2.13.0b20240423/src/waylay_sdk_registry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:43:58.000000 waylay_sdk_registry-2.13.0b20240423/src/waylay_sdk_registry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 07:43:58.000000 waylay_sdk_registry-2.13.0b20240423/src/waylay_sdk_registry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-24 07:43:58.000000 waylay_sdk_registry-2.13.0b20240423/src/waylay_sdk_registry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 07:43:58.000000 waylay_sdk_registry-2.13.0b20240423/src/waylay_sdk_registry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.831539 waylay-sdk-registry-2.13.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-03-29 13:21:52.831539 waylay-sdk-registry-2.13.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 13:21:52.831539 waylay-sdk-registry-2.13.0rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.823539 waylay-sdk-registry-2.13.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.823539 waylay-sdk-registry-2.13.0rc0/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.823539 waylay-sdk-registry-2.13.0rc0/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.823539 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.827539 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17657 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   167061 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/models_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   174919 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/plugs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    42593 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/runtimes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/schemas_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   168300 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/webscripts_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.827539 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/service/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.831539 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-03-29 13:21:52.000000 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-29 13:21:52.000000 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 13:21:52.000000 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-29 13:21:52.000000 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-29 13:21:52.000000 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-29 13:21:52.000000 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/top_level.txt
```

### Comparing `waylay_sdk_registry-2.13.0b20240423/LICENSE.txt` & `waylay-sdk-registry-2.13.0rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry-2.13.0b20240423/PKG-INFO` & `waylay-sdk-registry-2.13.0rc0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-registry
-Version: 2.13.0b20240423
+Version: 2.13.0rc0
 Summary: Waylay Function Registry
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,22 +13,21 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-registry-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/registry.html
 Keywords: Waylay Function Registry
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.1
+Requires-Dist: waylay-sdk~=0.0.4rc5
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -46,52 +45,57 @@
 Provides-Extra: types
 Requires-Dist: waylay-sdk-registry-types; extra == "types"
 
 # Waylay Registry Service
 V2 API to build and deploy Waylay functions (plugs, webscripts, BYOML models).
 
 This Python package is automatically generated based on the 
-Waylay Registry OpenAPI specification (API version: 2.13.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/registry.html).
+Waylay Registry OpenAPI specification (API version: 2.13.0-beta.0)
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Registry api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Registry api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-registry-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-registry is included in:
-- ```pip install waylay-sdk-core[registry]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[registry]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-registry and waylay-sdk-registry-types are included in:
-- ```pip install waylay-sdk-core[registry,registry-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[registry,registry-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-registry-types` is installed
-from waylay.services.registry.models.root_page_response import RootPageResponse
+from registry.models.function_type import FunctionType
+from registry.models.job_state_result import JobStateResult
+from registry.models.job_type_schema import JobTypeSchema
+from registry.models.jobs_response import JobsResponse
 try:
-    # Get Service Status
-    # calls `GET /registry/v2/`
-    api_response = await waylay_client.registry.about.get(
+    # List Jobs
+    # calls `GET /registry/v2/jobs/`
+    api_response = await waylay_client.registry.jobs.list(
+        # query parameters:
+        query = {
+        },
     )
-    print("The response of registry.about.get:\n")
+    print("The response of registry.jobs.list:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling registry.about.get: %s\n" % e)
+    print("Exception when calling registry.jobs.list: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_registry-2.13.0b20240423/README.md` & `waylay-sdk-registry-2.13.0rc0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 # Waylay Registry Service
 V2 API to build and deploy Waylay functions (plugs, webscripts, BYOML models).
 
 This Python package is automatically generated based on the 
-Waylay Registry OpenAPI specification (API version: 2.13.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/registry.html).
+Waylay Registry OpenAPI specification (API version: 2.13.0-beta.0)
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Registry api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Registry api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-registry-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-registry is included in:
-- ```pip install waylay-sdk-core[registry]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[registry]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-registry and waylay-sdk-registry-types are included in:
-- ```pip install waylay-sdk-core[registry,registry-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[registry,registry-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-registry-types` is installed
-from waylay.services.registry.models.root_page_response import RootPageResponse
+from registry.models.function_type import FunctionType
+from registry.models.job_state_result import JobStateResult
+from registry.models.job_type_schema import JobTypeSchema
+from registry.models.jobs_response import JobsResponse
 try:
-    # Get Service Status
-    # calls `GET /registry/v2/`
-    api_response = await waylay_client.registry.about.get(
+    # List Jobs
+    # calls `GET /registry/v2/jobs/`
+    api_response = await waylay_client.registry.jobs.list(
+        # query parameters:
+        query = {
+        },
     )
-    print("The response of registry.about.get:\n")
+    print("The response of registry.jobs.list:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling registry.about.get: %s\n" % e)
+    print("Exception when calling registry.jobs.list: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_registry-2.13.0b20240423/pyproject.toml` & `waylay-sdk-registry-2.13.0rc0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-registry"
-version = "2.13.0b20240423"
+version = "2.13.0rc0"
 description = "Waylay Function Registry"
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Function Registry"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk-core ~= 0.2.1",
+    "waylay-sdk ~= 0.0.4rc5",
     "pydantic ~= 2.6",
     "typing-extensions ~= 4.10",
     "eval-type-backport ~= 0.1.3; python_version < '3.10'",
 ]
 readme = "README.md"
 license={file = "LICENSE.txt"}
 
 [project.urls]
 Homepage = "https://www.waylay.io/"
-Documentation = "https://docs.waylay.io/#/api/?id=software-development-kits"
+Documentation = "https://docs.waylay.io/#/"
 Repository = "https://github.com/waylayio/waylay-sdk-registry-py.git"
-"Openapi Specification" = "https://docs.waylay.io/openapi/public/redocly/registry.html"
 
 [project.optional-dependencies]
 dev = [
     "mypy",
     "ruff",
     "types-python-jose",
     "types-appdirs",
```

### Comparing `waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/api/about_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/default_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,35 +29,35 @@
     Response,
 )
 from waylay.sdk.api._models import Model
 from waylay.sdk.plugin import WithApiClient
 
 if TYPE_CHECKING:
     from waylay.services.registry.models import RootPageResponse
-    from waylay.services.registry.queries.about_api import GetQuery
+    from waylay.services.registry.queries.default_api import GetQuery
 
 
 try:
     from waylay.services.registry.models import RootPageResponse
-    from waylay.services.registry.queries.about_api import GetQuery
+    from waylay.services.registry.queries.default_api import GetQuery
 
     MODELS_AVAILABLE = True
 except ImportError:
     MODELS_AVAILABLE = False
 
     if not TYPE_CHECKING:
         GetQuery = dict
         RootPageResponse = Model
 
 
 T = TypeVar("T")
 
 
-class AboutApi(WithApiClient):
-    """AboutApi service methods.
+class DefaultApi(WithApiClient):
+    """DefaultApi service methods.
 
     NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -65,92 +65,85 @@
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> RootPageResponse: ...
 
     @overload
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> RootPageResponse | T | Response | Model:
-        """Get Service Status.
+        """Version.
 
-        Get the status and version of the function registry service.
+        Get the version of this function registry deployment.
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -161,22 +154,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "*": RootPageResponse if not select_path else Model,
```

### Comparing `waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/api/jobs_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/jobs_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 """
 
 from __future__ import annotations  # for Python 3.7–3.9
 
 from typing import (
     TYPE_CHECKING,
     Any,
-    AsyncIterator,
     Dict,
     Literal,
     TypeVar,
     overload,
 )
 
 from pydantic import (
@@ -27,15 +26,14 @@
 )
 from waylay.sdk.api import (
     HeaderTypes,
     QueryParamTypes,
     Response,
 )
 from waylay.sdk.api._models import Model
-from waylay.sdk.api.constants import STREAM_TIMEOUTS
 from waylay.sdk.plugin import WithApiClient
 
 if TYPE_CHECKING:
     from waylay.services.registry.models import (
         EventWithCloseSSE,
         JobResponse,
         JobsResponse,
@@ -93,99 +91,76 @@
     async def events(
         self,
         *,
         query: EventsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[EventWithCloseSSE]: ...
+    ) -> EventWithCloseSSE: ...
 
     @overload
     async def events(
         self,
         *,
         query: EventsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[T]: ...
+    ) -> T: ...
 
     @overload
     async def events(
         self,
         *,
         query: EventsQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def events(
         self,
         *,
         query: EventsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[Model]: ...
+    ) -> Model: ...
 
     @overload
     async def events(
         self,
         *,
         query: EventsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[T]: ...
+    ) -> T: ...
 
     async def events(
         self,
         *,
         query: EventsQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> (
-        AsyncIterator[EventWithCloseSSE]
-        | AsyncIterator[T]
-        | Response
-        | AsyncIterator[Model]
-    ):
+    ) -> EventWithCloseSSE | T | Response | Model:
         """Stream Events.
 
         Get an SSE stream of all job events for the users tenant.  The stream can be filtered on job type or on a specific job id.   When filtering on job id, the server will send a <code>close</code> event  upon completion of the job. The client should handle this event by closing the stream.
         :param query: URL Query parameters.
         :type query: EventsQuery | QueryParamTypes, optional
         :param query['type'] (dict) <br> query.type (Query) : The type of the job.
         :type query['type']: JobType
@@ -193,15 +168,14 @@
         :type query['id']: str
         :param query['children'] (dict) <br> query.children (Query) : If set to <code>true</code>, the event stream will include events of the job's dependants. E.g., when subscribing to a verify job with `children=true`, you will also receive the events of the underlying build and deploy jobs. Defaults to <code>false</code>.
         :type query['children']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -212,22 +186,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(EventsQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": EventWithCloseSSE if not select_path else Model,
@@ -240,16 +218,14 @@
         return await self.api_client.request(
             method="GET",
             resource_path="/registry/v2/jobs/events",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
-            stream=stream,
-            timeout=timeout,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
@@ -258,89 +234,83 @@
         type: JobType,
         id: StrictStr,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> JobResponse: ...
 
     @overload
     async def get(
         self,
         type: JobType,
         id: StrictStr,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get(
         self,
         type: JobType,
         id: StrictStr,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get(
         self,
         type: JobType,
         id: StrictStr,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get(
         self,
         type: JobType,
         id: StrictStr,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get(
         self,
         type: JobType,
         id: StrictStr,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> JobResponse | T | Response | Model:
         """Get Job.
 
         Get a background job by type and id.
         :param type: (required)
@@ -349,15 +319,14 @@
         :type id: str
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -368,25 +337,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "type": str(type),
             "id": str(id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": JobResponse if not select_path else Model,
@@ -413,79 +386,73 @@
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> JobsResponse: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> JobsResponse | T | Response | Model:
         """List Jobs.
 
         List all background jobs for the users tenant.
         :param query: URL Query parameters.
@@ -502,15 +469,14 @@
         :type query['createdBefore']: TimestampSpec
         :param query['createdAfter'] (dict) <br> query.created_after (Query) : Filter on jobs that created after the given timestamp or age
         :type query['createdAfter']: TimestampSpec
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -521,22 +487,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(ListQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": JobsResponse if not select_path else Model,
```

### Comparing `waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/api/models_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/models_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -230,15 +230,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostModelJobSyncResponseV2 | PostModelJobAsyncResponseV2: ...
 
     @overload
     async def create(
         self,
@@ -258,15 +257,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def create(
         self,
@@ -286,15 +284,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def create(
         self,
@@ -314,15 +311,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def create(
         self,
@@ -342,15 +338,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def create(
         self,
         *,
@@ -369,15 +364,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> (
         PostModelJobSyncResponseV2 | PostModelJobAsyncResponseV2 | T | Response | Model
     ):
         """Create Model.
 
@@ -386,43 +380,40 @@
         :type json: bytearray, optional
         :param content: The assets for a <em>model</em> function can be provided as   <ul>     <li>A single <em>tar</em> archive (optionally compressed), with one of the content types      <code>application/octet-stream</code>, <code>application/tar</code>, <code>application/tar+gzip</code>, <code>application/x-gzip</code>, <code>application/x-tar</code>, <code>application/gzip</code></li>     <li>Separate files in a <code>multipart/form-data</code> request</li>     <li>A reference to the assets of another <em>model</em> in the <code>copy</code> argument</li>   </ul>    The required <code>model.json</code> json file contains the function metadata,   and must have a <code>runtime</code> attribute that is one of the supported <em>runtime</em>s    (see <code>GET /registry/v2/runtimes?functionType=kfserving</code>).    For each <em>runtime</em> other files will be required or supported.
         :type content: ContentRequest, optional
         :param files: The files of a `content-type: multipart/form-data` request.
         :type files: FilesRequest, optional
         :param query: URL Query parameters.
         :type query: CreateQuery | QueryParamTypes, optional
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
         :param query['deprecatePrevious'] (dict) <br> query.deprecate_previous (Query) : Set the cleanup policy used to automatically deprecate/delete previous versions.
         :type query['deprecatePrevious']: DeprecatePreviousPolicy
         :param query['dryRun'] (dict) <br> query.dry_run (Query) : If set to <code>true</code>, validates the deployment conditions, but does not change anything.
         :type query['dryRun']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
+        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. Saves computing resources when the function is not to be used immediately.
+        :type query['scaleToZero']: bool
         :param query['version'] (dict) <br> query.version (Query) : If set, the function version will be an increment of the latest existing version that satisfies the `version` range. Note that this increment always takes precedence over an explicit `version` in the function manifest.
         :type query['version']: SemanticVersionRange
         :param query['name'] (dict) <br> query.name (Query) : If set, the value will be used as the function name instead of the one specified in the manifest.
         :type query['name']: str
         :param query['draft'] (dict) <br> query.draft (Query) : If set, the created function will be a draft function and its assets are still mutable. A build and deploy is initiated only in the case when all necessary assets are present and valid.
         :type query['draft']: bool
         :param query['runtime'] (dict) <br> query.runtime (Query) : If set, the created function will use the indicated runtime (latest version within specified range).  This takes precedence over the runtime specified in a function manifest (copied or from request body).
         :type query['runtime']: str
         :param query['copy'] (dict) <br> query.copy_from (Query) : Indicates the _source_ of initial assets for a _new function_.  When using this query parameter, the request body does not need to contain assets, but any assets in the request body will overwrite the copied assets.  #### Selection of _assets_ source  * If set as `<sourceName>[@<sourceVersionRange>]`, the _new function_ will be created with copied assets of the selected _source function_. * If set as `!example`, a `runtime` query parameter is required, and the _new function_ will be initialized with assets of the _runtime example_.  #### Selection of the _source function_  When `<sourceVersionRange>` is a range (or is not given), the latest _published_ version (in that range) is used.  If no _published_ version exists, the latest _draft_ is selected.  If no versions in the range exist, a `404` _Not Found_ error is returned.  #### The `name` of the _new function_  If a `name` is NOT specified (either as query parameter, or in an optional manifest asset in the request body), the `name` of the _new function_ will be that of the _source function_.  #### The `version` of the _new function_  When the _target_ and _source_ name are equal, the `version` query parameters is defaulted to `<sourceVersionRange>` (`~<sourceVersionRange>` when it's an exact version)  The version of the _new function_ will be: * If a `version` is NOT specified (either as query parameter, in an optional manifest asset, or as `<sourceVersionRange>` _default_)    * a **patch increment** (`<major>.<minor>.<patch>+1`) of the latest **existing version** with the target `name`    * **`1.0.0`** otherwise  * If a `version` is specified:    * the **lowest version** in that range **if no existing version** is in that range.    * an **increment** of the latest existing version, **at the highest level** (_major_,_minor_,_patch_) allowed by that range.    * otherwise, if all allowed versions already exist, a **`409` _Duplicate_ error** is raised.  #### Deployment overrides  The new function will use the deployment overrides of the copied function, unless a _manifest_ was specified in the request body.
         :type query['copy']: CreateWebscriptsCopyParameter
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -433,35 +424,39 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
+        if json is not None and should_validate:
             body_adapter = TypeAdapter(
                 Annotated[
                     Optional[Union[StrictBytes, StrictStr]],
                     Field(
                         description="The assets for a <em>model</em> function can be provided as   <ul>     <li>A single <em>tar</em> archive (optionally compressed), with one of the content types      <code>application/octet-stream</code>, <code>application/tar</code>, <code>application/tar+gzip</code>, <code>application/x-gzip</code>, <code>application/x-tar</code>, <code>application/gzip</code></li>     <li>Separate files in a <code>multipart/form-data</code> request</li>     <li>A reference to the assets of another <em>model</em> in the <code>copy</code> argument</li>   </ul>    The required <code>model.json</code> json file contains the function metadata,   and must have a <code>runtime</code> attribute that is one of the supported <em>runtime</em>s    (see <code>GET /registry/v2/runtimes?functionType=kfserving</code>).    For each <em>runtime</em> other files will be required or supported. "
                     ),
                 ]
             )
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
         body_args["content"] = content
         body_args["files"] = files
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(CreateQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": PostModelJobSyncResponseV2 if not select_path else Model,
@@ -499,15 +494,14 @@
             ),
         ],
         *,
         query: DeleteAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostModelJobSyncResponseV2 | PostModelJobAsyncResponseV2: ...
 
     @overload
     async def delete_asset(
         self,
@@ -522,15 +516,14 @@
             ),
         ],
         *,
         query: DeleteAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def delete_asset(
         self,
@@ -545,15 +538,14 @@
             ),
         ],
         *,
         query: DeleteAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def delete_asset(
         self,
@@ -568,15 +560,14 @@
             ),
         ],
         *,
         query: DeleteAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def delete_asset(
         self,
@@ -591,15 +582,14 @@
             ),
         ],
         *,
         query: DeleteAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def delete_asset(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -613,15 +603,14 @@
             ),
         ],
         *,
         query: DeleteAssetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> (
         PostModelJobSyncResponseV2 | PostModelJobAsyncResponseV2 | T | Response | Model
     ):
         """Delete Model Asset.
 
@@ -630,31 +619,26 @@
         :type name: str
         :param version: The version of the function. (required)
         :type version: str
         :param wildcard: Full path or path prefix of the asset within the archive (required)
         :type wildcard: str
         :param query: URL Query parameters.
         :type query: DeleteAssetQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['chown'] (dict) <br> query.chown (Query) : If set, ownership of the draft function is transferred to the current user.
         :type query['chown']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -665,26 +649,30 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
             "wildcard": str(wildcard),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(DeleteAssetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": PostModelJobSyncResponseV2 if not select_path else Model,
@@ -718,15 +706,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> bytearray: ...
 
     @overload
     async def get_archive(
         self,
@@ -735,15 +722,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get_archive(
         self,
@@ -752,15 +738,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get_archive(
         self,
@@ -769,15 +754,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get_archive(
         self,
@@ -786,15 +770,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get_archive(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -802,15 +785,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetArchiveQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> bytearray | T | Response | Model:
         """Get Model Archive.
 
         Get the specification archive of a model.
         :param name: The name of the function. (required)
@@ -821,15 +803,14 @@
         :type query: GetArchiveQuery | QueryParamTypes, optional
         :param query['ls'] (dict) <br> query.ls (Query) : If set to `true`, the result will be a listing of the files in the asset, annotated with metadata and validation report from the asset conditions of the functions runtime.
         :type query['ls']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -840,25 +821,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetArchiveQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": bytearray if not select_path else Model,
@@ -895,15 +880,14 @@
             ),
         ],
         *,
         query: GetAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> bytearray: ...
 
     @overload
     async def get_asset(
         self,
@@ -918,15 +902,14 @@
             ),
         ],
         *,
         query: GetAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get_asset(
         self,
@@ -941,15 +924,14 @@
             ),
         ],
         *,
         query: GetAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get_asset(
         self,
@@ -964,15 +946,14 @@
             ),
         ],
         *,
         query: GetAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get_asset(
         self,
@@ -987,15 +968,14 @@
             ),
         ],
         *,
         query: GetAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get_asset(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -1009,15 +989,14 @@
             ),
         ],
         *,
         query: GetAssetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> bytearray | T | Response | Model:
         """Get File From Model Archive.
 
         Get a file from the specification archive of a model.
         :param name: The name of the function. (required)
@@ -1030,15 +1009,14 @@
         :type query: GetAssetQuery | QueryParamTypes, optional
         :param query['ls'] (dict) <br> query.ls (Query) : If set to `true`, the result will be a listing of the files in the asset, annotated with metadata and validation report from the asset conditions of the functions runtime.
         :type query['ls']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1049,26 +1027,30 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
             "wildcard": str(wildcard),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetAssetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": bytearray if not select_path else Model,
@@ -1096,84 +1078,78 @@
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetModelResponseV2: ...
 
     @overload
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetModelResponseV2 | T | Response | Model:
         """Get Latest Model Version.
 
         Fetch the latest version of a <em>model</em>.    By default, the result shows the latest non-deprecated, non-draft version.   If there is no such version, the latest deprecated or the latest draft version is returned, with the former taking precedence.       Use the boolean query parameters <code>includeDeprecated</code> or <code>includeDraft</code> to change this behaviour:   <ul>   <li><code>includeDeprecated=true</code>: do not prefer non-deprecated versions as a latest version: if the latest version is a deprecated one, it will be shown, even if there are older non-deprecated versions.</li>   <li><code>includeDraft=true</code>: do not prefer non-draft versions as a latest version: if the latest version is a draft, it will be shown, even if there are older non-draft versions.</li>   </ul>     The returned <em>model version</em> will contain a link to its   latest _draft_ or latest _published_ version (if existing and different).
         :param name: The name of the function. (required)
@@ -1184,15 +1160,14 @@
         :type query['includeDraft']: bool
         :param query['includeDeprecated'] (dict) <br> query.include_deprecated (Query) : Configures the inclusion of _deprecated_ versions when selecting latest versions per name. By default, deprecated versions are only considered when no other versions are available. If set to `true`, deprecated versions are **included**. If set to `false`, deprecated versions are **excluded**.
         :type query['includeDeprecated']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1203,24 +1178,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetLatestQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": GetModelResponseV2 if not select_path else Model,
@@ -1251,15 +1230,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetModelResponseV2: ...
 
     @overload
     async def get(
         self,
@@ -1268,15 +1246,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get(
         self,
@@ -1285,15 +1262,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get(
         self,
@@ -1302,15 +1278,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get(
         self,
@@ -1319,15 +1294,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -1335,15 +1309,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetModelResponseV2 | T | Response | Model:
         """Get Model Version.
 
         Get a model by name and version.
         :param name: The name of the function. (required)
@@ -1352,15 +1325,14 @@
         :type version: str
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1371,25 +1343,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": GetModelResponseV2 if not select_path else Model,
@@ -1420,15 +1396,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: JobsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> JobsForModelResponseV2: ...
 
     @overload
     async def jobs(
         self,
@@ -1437,15 +1412,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: JobsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def jobs(
         self,
@@ -1454,15 +1428,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: JobsQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def jobs(
         self,
@@ -1471,15 +1444,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: JobsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def jobs(
         self,
@@ -1488,15 +1460,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: JobsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def jobs(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -1504,15 +1475,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: JobsQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> JobsForModelResponseV2 | T | Response | Model:
         """List Model Jobs.
 
         List the ongoing and completed operations on a model.
         :param name: The name of the function. (required)
@@ -1533,15 +1503,14 @@
         :type query['createdBefore']: TimestampSpec
         :param query['createdAfter'] (dict) <br> query.created_after (Query) : Filter on jobs that created after the given timestamp or age
         :type query['createdAfter']: TimestampSpec
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1552,25 +1521,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(JobsQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": JobsForModelResponseV2 if not select_path else Model,
@@ -1597,79 +1570,73 @@
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> LatestModelsResponseV2: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> LatestModelsResponseV2 | T | Response | Model:
         """List Models.
 
         List the (latest) versions of available <em>models</em>.  ### List Latest Model Versions By default, the result includes the latest non-deprecated, non-draft version for each <em>model</em> name. If there is no such version, the latest _deprecated_ or the latest _draft_ version is included, with the former taking precedence.     Use the boolean query parameters <code>includeDeprecated</code> or <code>includeDraft</code> to change this behaviour:   <ul>   <li><code>includeDeprecated=true</code>: do not prefer non-deprecated versions as a latest version: if the latest version is a deprecated one, it will be shown, even if there are older non-deprecated versions.</li>   <li><code>includeDraft=true</code>: do not prefer non-draft versions as a latest version: if the latest version is a draft, it will be shown, even if there are older non-draft versions.</li>   </ul>   As long as no version filters are used, each listed <em>model version</em> contains representations of the latest draft (`entities[]._links.draft`)  or latest published (`entities[]._links.published`) version (if existing and different).   Use the query parameter `showRelated` to include only a link (default `showRelated=link`) or a full representation (`showRelated=embed`).  ### List Latest Model Versions (with filter) When any of the _version filter_ query parameters are used, the response contains the _latest_ version per named <em>model</em> that satisfy the filters, but **without links**.  ### List All Model Versions When using `latest=false` (default when using the `namedVersion` filter), the listing contains _all_  <em>models</em> versions that satisfy the query, possibly multiple versions per named <em>models</em>. No HAL links are provided.  #### Filter on _status_ By default <em>model versions</em> with status  `undeployed` are **excluded** in all cases. Use the _version filter_ `status` to include/exclude a status from the results. By example,  > `?status=any&includeDeprecated=true&includeDraft=true&latest=false`  will list _ALL_ versions known to the function registry.  #### Version filter parameters The following query parameters are _version filters_ for the <em>model</em> listing: > `version`, `status`, `runtimeVersion`, `createdBy`, `createdBefore`, `createdAfter`, `updatedBy`, `updatedBefore`, `updatedAfter`, `nameVersion`, `deprecated`, `draft`
         :param query: URL Query parameters.
@@ -1716,15 +1683,14 @@
         :type query['latest']: bool
         :param query['showRelated'] (dict) <br> query.show_related (Query) : Sets the representation of related function versions (like the _latest_ draft and/or published) in the response. - `embed`: as full summary representation (in `_embedded`). - `link`: as HAL link in (in `_links`). - `none`: omitted.
         :type query['showRelated']: ShowRelatedType
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1735,22 +1701,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(ListQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": LatestModelsResponseV2 if not select_path else Model,
@@ -1778,84 +1748,78 @@
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ModelVersionsResponseV2: ...
 
     @overload
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ModelVersionsResponseV2 | T | Response | Model:
         """List Model Versions.
 
         List all deployed versions of a model.
         :param name: The name of the function. (required)
@@ -1892,15 +1856,14 @@
         :type query['archiveFormat']: List[ArchiveFormat]
         :param query['runtime'] (dict) <br> query.runtime (Query) : Filter on the runtime of the function.
         :type query['runtime']: List[str]
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1911,24 +1874,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(ListVersionsQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": ModelVersionsResponseV2 if not select_path else Model,
@@ -1960,15 +1927,14 @@
         ],
         *,
         json: FunctionMeta | None = None,
         query: PatchMetadataQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetModelResponseV2: ...
 
     @overload
     async def patch_metadata(
         self,
@@ -1978,15 +1944,14 @@
         ],
         *,
         json: FunctionMeta | None = None,
         query: PatchMetadataQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def patch_metadata(
         self,
@@ -1996,15 +1961,14 @@
         ],
         *,
         json: FunctionMeta | None = None,
         query: PatchMetadataQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def patch_metadata(
         self,
@@ -2014,15 +1978,14 @@
         ],
         *,
         json: FunctionMeta | None = None,
         query: PatchMetadataQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def patch_metadata(
         self,
@@ -2032,15 +1995,14 @@
         ],
         *,
         json: FunctionMeta | None = None,
         query: PatchMetadataQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def patch_metadata(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -2049,15 +2011,14 @@
         ],
         *,
         json: FunctionMeta | None = None,
         query: PatchMetadataQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetModelResponseV2 | T | Response | Model:
         """Patch Model Metadata.
 
         Patch the metadata of a model version.
         :param name: The name of the function. (required)
@@ -2070,15 +2031,14 @@
         :type query: PatchMetadataQuery | QueryParamTypes, optional
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -2089,29 +2049,33 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
+        if json is not None and should_validate:
             body_adapter = TypeAdapter(Optional[FunctionMeta])
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(PatchMetadataQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": GetModelResponseV2 if not select_path else Model,
@@ -2142,15 +2106,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: PublishQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostModelJobSyncResponseV2 | PostModelJobAsyncResponseV2: ...
 
     @overload
     async def publish(
         self,
@@ -2159,15 +2122,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: PublishQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def publish(
         self,
@@ -2176,15 +2138,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: PublishQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def publish(
         self,
@@ -2193,15 +2154,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: PublishQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def publish(
         self,
@@ -2210,15 +2170,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: PublishQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def publish(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -2226,15 +2185,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: PublishQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> (
         PostModelJobSyncResponseV2 | PostModelJobAsyncResponseV2 | T | Response | Model
     ):
         """Publish Draft Model.
 
@@ -2255,15 +2213,14 @@
         :type query['deprecatePrevious']: DeprecatePreviousPolicy
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -2274,25 +2231,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(PublishQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": PostModelJobSyncResponseV2 if not select_path else Model,
@@ -2324,15 +2285,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RebuildQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> RebuildModelSyncResponseV2 | RebuildModelAsyncResponseV2: ...
 
     @overload
     async def rebuild(
         self,
@@ -2341,15 +2301,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RebuildQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def rebuild(
         self,
@@ -2358,15 +2317,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RebuildQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def rebuild(
         self,
@@ -2375,15 +2333,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RebuildQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def rebuild(
         self,
@@ -2392,15 +2349,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RebuildQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def rebuild(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -2408,50 +2364,48 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RebuildQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> (
         RebuildModelSyncResponseV2 | RebuildModelAsyncResponseV2 | T | Response | Model
     ):
         """Rebuild Model.
 
         Rebuild and deploy a model with the original or updated base image.
         :param name: The name of the function. (required)
         :type name: str
         :param version: The version of the function. (required)
         :type version: str
         :param query: URL Query parameters.
         :type query: RebuildQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.
-        :type query['scaleToZero']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['dryRun'] (dict) <br> query.dry_run (Query) : If set to <code>true</code>, checks whether rebuild jobs are needed, but do not start any jobs.
         :type query['dryRun']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param query['upgrade'] (dict) <br> query.upgrade (Query) : If set, force a rebuild with the given <em>runtime</em> version selection policy. <ul>  <li><code>same</code> <b>patch</b> version.   This should only include backward compatible upgrades.  </li>  <li><code>minor</code> <b>major</b> version.   This might include an upgrade of e.g. the language runtime and/or provided   dependencies that could break compatiblity with the function. .</li> </ul>
         :type query['upgrade']: RebuildPolicy
         :param query['forceVersion'] (dict) <br> query.force_version (Query) : If set, force a rebuild with the given runtime version (including downgrades). This parameter is mutually exclusive to the `upgrade` parameter.
         :type query['forceVersion']: str
         :param query['ignoreChecks'] (dict) <br> query.ignore_checks (Query) : If set to true, checks that normally prevent a rebuild are overriden. These checks include: * function state in `pending`, `running`, `failed` or `undeployed` * backoff period due to recent failures * usage of deprecated dependencies * running jobs on entity * the `dryRun` option
         :type query['ignoreChecks']: bool
+        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful (re-)deployment. If not set, the function is scaled to zero only if it was not active before this command.
+        :type query['scaleToZero']: bool
         :param query['skipRebuild'] (dict) <br> query.skip_rebuild (Query) : If set, the function will not be rebuild. Always uses the current runtime version when re-deploying/re-verifying the function.
         :type query['skipRebuild']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -2462,25 +2416,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(RebuildQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": RebuildModelSyncResponseV2 if not select_path else Model,
@@ -2512,15 +2470,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RemoveVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> UndeployedResponseV2 | UndeploySubmittedResponseV2: ...
 
     @overload
     async def remove_version(
         self,
@@ -2529,15 +2486,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RemoveVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def remove_version(
         self,
@@ -2546,15 +2502,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RemoveVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def remove_version(
         self,
@@ -2563,15 +2518,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RemoveVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def remove_version(
         self,
@@ -2580,15 +2534,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RemoveVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def remove_version(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -2596,15 +2549,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RemoveVersionQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> UndeployedResponseV2 | UndeploySubmittedResponseV2 | T | Response | Model:
         """Remove Model Version.
 
         Deprecate, undeploy and/or remove a <em>model</em> version.    By default, a `DELETE`    * _deprecates_ the model version(s): they are no longer included in listings by default.   * _undeploys_ the model version(s) with delay: the function can no longer be invoked, the small delay allows     other services to discover the removal.   * _removes_ the version(s) from the plug registry.    Use `?force=true` to immediately _undeploy_ and _remove_ without delay.    Use `?undeploy=true` to undeploy, but keep the model version registered in a `undeployed` state.   An `undeployed` version can later be restored by a _rebuild_ action.
         :param name: The name of the function. (required)
@@ -2621,15 +2573,14 @@
         :type query['force']: bool
         :param query['undeploy'] (dict) <br> query.undeploy (Query) : If `true`, the `DELETE` operation * undeploys the (openfaas) function: it becomes no longer available for invocation. * does NOT remove the function from registry: it stays in an `undeployed` status.  All assets and definitions are retained, so the version can be restored later with a  _rebuild_ action.  If `false`, the `DELETE` operation * _only_ marks the plug function as _deprecated_, the function remains active but is removed from the default listings.   This also applies to _draft_ versions.  This parameter is incompatible with `force=true`.  If not set the default behaviour applies: * _draft_ versions are _undeployed_ and _removed_ from registry. * non-_draft_ versions are marked _deprecated_ only.
         :type query['undeploy']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -2640,25 +2591,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(RemoveVersionQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": UndeployedResponseV2 if not select_path else Model,
@@ -2687,84 +2642,78 @@
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: RemoveVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> UndeployedResponseV2 | UndeploySubmittedResponseV2: ...
 
     @overload
     async def remove_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: RemoveVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def remove_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: RemoveVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def remove_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: RemoveVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def remove_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: RemoveVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def remove_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: RemoveVersionsQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> UndeployedResponseV2 | UndeploySubmittedResponseV2 | T | Response | Model:
         """Remove Model.
 
         Deprecate, undeploy and/or remove all versions of this named <em>model</em>.    By default, a `DELETE`    * _deprecates_ the model version(s): they are no longer included in listings by default.   * _undeploys_ the model version(s) with delay: the function can no longer be invoked, the small delay allows     other services to discover the removal.   * _removes_ the version(s) from the plug registry.    Use `?force=true` to immediately _undeploy_ and _remove_ without delay.    Use `?undeploy=true` to undeploy, but keep the model version registered in a `undeployed` state.   An `undeployed` version can later be restored by a _rebuild_ action.
         :param name: The name of the function. (required)
@@ -2779,15 +2728,14 @@
         :type query['undeploy']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -2798,24 +2746,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(RemoveVersionsQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": UndeployedResponseV2 if not select_path else Model,
@@ -2856,15 +2808,14 @@
         content: Annotated[
             RequestContent | None, Field(description="A single asset file.")
         ] = None,
         query: UpdateAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostModelJobSyncResponseV2 | PostModelJobAsyncResponseV2: ...
 
     @overload
     async def update_asset(
         self,
@@ -2882,15 +2833,14 @@
         content: Annotated[
             RequestContent | None, Field(description="A single asset file.")
         ] = None,
         query: UpdateAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def update_asset(
         self,
@@ -2908,15 +2858,14 @@
         content: Annotated[
             RequestContent | None, Field(description="A single asset file.")
         ] = None,
         query: UpdateAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def update_asset(
         self,
@@ -2934,15 +2883,14 @@
         content: Annotated[
             RequestContent | None, Field(description="A single asset file.")
         ] = None,
         query: UpdateAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def update_asset(
         self,
@@ -2960,15 +2908,14 @@
         content: Annotated[
             RequestContent | None, Field(description="A single asset file.")
         ] = None,
         query: UpdateAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def update_asset(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -2985,15 +2932,14 @@
         content: Annotated[
             RequestContent | None, Field(description="A single asset file.")
         ] = None,
         query: UpdateAssetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> (
         PostModelJobSyncResponseV2 | PostModelJobAsyncResponseV2 | T | Response | Model
     ):
         """Update Model Asset.
 
@@ -3004,31 +2950,26 @@
         :type version: str
         :param wildcard: Full path or path prefix of the asset within the archive (required)
         :type wildcard: str
         :param content: A single asset file.
         :type content: ContentRequest, optional
         :param query: URL Query parameters.
         :type query: UpdateAssetQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['chown'] (dict) <br> query.chown (Query) : If set, ownership of the draft function is transferred to the current user.
         :type query['chown']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -3039,27 +2980,31 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
             "wildcard": str(wildcard),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
         body_args["content"] = content
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(UpdateAssetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": PostModelJobSyncResponseV2 if not select_path else Model,
@@ -3102,15 +3047,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: UpdateAssetsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostModelJobSyncResponseV2 | PostModelJobAsyncResponseV2: ...
 
     @overload
     async def update_assets(
         self,
@@ -3128,15 +3072,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: UpdateAssetsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def update_assets(
         self,
@@ -3154,15 +3097,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: UpdateAssetsQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def update_assets(
         self,
@@ -3180,15 +3122,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: UpdateAssetsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def update_assets(
         self,
@@ -3206,15 +3147,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: UpdateAssetsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def update_assets(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -3231,15 +3171,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: UpdateAssetsQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> (
         PostModelJobSyncResponseV2 | PostModelJobAsyncResponseV2 | T | Response | Model
     ):
         """Update Model Assets.
 
@@ -3250,31 +3189,26 @@
         :type version: str
         :param content: The assets for a <em>model</em> function can be provided as either   <ul>     <li>a single <em>tar</em> archive (optionally compressed), with one of the content types      <code>application/octet-stream</code>, <code>application/tar</code>, <code>application/tar+gzip</code>, <code>application/x-gzip</code>, <code>application/x-tar</code>, <code>application/gzip</code></li>     <li>separate files in a <code>multipart/form-data</code> request</li>   </ul>    The provided assets will be added to the <em>model</em> function's collection of existing assets,   replacing any existing assets with the same name.    Please note that it is not allowed to update the model.json</code> json file with a changed value for any of the    <code>name</code>, <code>version</code> and/or <code>runtime</code> attributes.    For each <em>runtime</em> other files are supported.
         :type content: ContentRequest, optional
         :param files: The files of a `content-type: multipart/form-data` request.
         :type files: FilesRequest, optional
         :param query: URL Query parameters.
         :type query: UpdateAssetsQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['chown'] (dict) <br> query.chown (Query) : If set, ownership of the draft function is transferred to the current user.
         :type query['chown']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -3285,27 +3219,31 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
         body_args["content"] = content
         body_args["files"] = files
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(UpdateAssetsQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": PostModelJobSyncResponseV2 if not select_path else Model,
@@ -3339,15 +3277,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: VerifyQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> VerifyModelSyncResponseV2 | PostModelJobAsyncResponseV2: ...
 
     @overload
     async def verify(
         self,
@@ -3356,15 +3293,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: VerifyQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def verify(
         self,
@@ -3373,15 +3309,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: VerifyQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def verify(
         self,
@@ -3390,15 +3325,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: VerifyQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def verify(
         self,
@@ -3407,15 +3341,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: VerifyQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def verify(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -3423,36 +3356,34 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: VerifyQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> VerifyModelSyncResponseV2 | PostModelJobAsyncResponseV2 | T | Response | Model:
         """Verify Health Of Model.
 
         Verify health of model deployed on openfaas.
         :param name: The name of the function. (required)
         :type name: str
         :param version: The version of the function. (required)
         :type version: str
         :param query: URL Query parameters.
         :type query: VerifyQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.
-        :type query['scaleToZero']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
+        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.
+        :type query['scaleToZero']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -3463,25 +3394,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(VerifyQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": VerifyModelSyncResponseV2 if not select_path else Model,
```

### Comparing `waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/api/plugs_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/plugs_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -239,15 +239,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostPlugJobSyncResponseV2 | PostPlugJobAsyncResponseV2: ...
 
     @overload
     async def create(
         self,
@@ -267,15 +266,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def create(
         self,
@@ -295,15 +293,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def create(
         self,
@@ -323,15 +320,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def create(
         self,
@@ -351,15 +347,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def create(
         self,
         *,
@@ -378,58 +373,54 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostPlugJobSyncResponseV2 | PostPlugJobAsyncResponseV2 | T | Response | Model:
         """Create Plug.
 
         Creates a new <em>plug</em> function by uploading its assets.      The assets for a <em>plug</em> function can be provided as   <ul>     <li>A single <em>tar</em> archive (optionally compressed), with one of the content types      <code>application/octet-stream</code>, <code>application/tar</code>, <code>application/tar+gzip</code>, <code>application/x-gzip</code>, <code>application/x-tar</code>, <code>application/gzip</code></li>     <li>Separate files in a <code>multipart/form-data</code> request</li>     <li>A reference to the assets of another <em>plug</em> in the <code>copy</code> argument</li>   </ul>    The required <code>plug.json</code> json file contains the function metadata,   and must have a <code>runtime</code> attribute that is one of the supported <em>runtime</em>s    (see <code>GET /registry/v2/runtimes?functionType=plugs</code>).    For each <em>runtime</em> other files will be required or supported.
         :param json: The assets for a <em>plug</em> function can be provided as   <ul>     <li>A single <em>tar</em> archive (optionally compressed), with one of the content types      <code>application/octet-stream</code>, <code>application/tar</code>, <code>application/tar+gzip</code>, <code>application/x-gzip</code>, <code>application/x-tar</code>, <code>application/gzip</code></li>     <li>Separate files in a <code>multipart/form-data</code> request</li>     <li>A reference to the assets of another <em>plug</em> in the <code>copy</code> argument</li>   </ul>    The required <code>plug.json</code> json file contains the function metadata,   and must have a <code>runtime</code> attribute that is one of the supported <em>runtime</em>s    (see <code>GET /registry/v2/runtimes?functionType=plugs</code>).    For each <em>runtime</em> other files will be required or supported.
         :type json: bytearray, optional
         :param content: The assets for a <em>plug</em> function can be provided as   <ul>     <li>A single <em>tar</em> archive (optionally compressed), with one of the content types      <code>application/octet-stream</code>, <code>application/tar</code>, <code>application/tar+gzip</code>, <code>application/x-gzip</code>, <code>application/x-tar</code>, <code>application/gzip</code></li>     <li>Separate files in a <code>multipart/form-data</code> request</li>     <li>A reference to the assets of another <em>plug</em> in the <code>copy</code> argument</li>   </ul>    The required <code>plug.json</code> json file contains the function metadata,   and must have a <code>runtime</code> attribute that is one of the supported <em>runtime</em>s    (see <code>GET /registry/v2/runtimes?functionType=plugs</code>).    For each <em>runtime</em> other files will be required or supported.
         :type content: ContentRequest, optional
         :param files: The files of a `content-type: multipart/form-data` request.
         :type files: FilesRequest, optional
         :param query: URL Query parameters.
         :type query: CreateQuery | QueryParamTypes, optional
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
         :param query['deprecatePrevious'] (dict) <br> query.deprecate_previous (Query) : Set the cleanup policy used to automatically deprecate/delete previous versions.
         :type query['deprecatePrevious']: DeprecatePreviousPolicy
         :param query['dryRun'] (dict) <br> query.dry_run (Query) : If set to <code>true</code>, validates the deployment conditions, but does not change anything.
         :type query['dryRun']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
+        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. Saves computing resources when the function is not to be used immediately.
+        :type query['scaleToZero']: bool
         :param query['version'] (dict) <br> query.version (Query) : If set, the function version will be an increment of the latest existing version that satisfies the `version` range. Note that this increment always takes precedence over an explicit `version` in the function manifest.
         :type query['version']: SemanticVersionRange
         :param query['name'] (dict) <br> query.name (Query) : If set, the value will be used as the function name instead of the one specified in the manifest.
         :type query['name']: str
         :param query['draft'] (dict) <br> query.draft (Query) : If set, the created function will be a draft function and its assets are still mutable. A build and deploy is initiated only in the case when all necessary assets are present and valid.
         :type query['draft']: bool
         :param query['runtime'] (dict) <br> query.runtime (Query) : If set, the created function will use the indicated runtime (latest version within specified range).  This takes precedence over the runtime specified in a function manifest (copied or from request body).
         :type query['runtime']: str
         :param query['copy'] (dict) <br> query.copy_from (Query) : Indicates the _source_ of initial assets for a _new function_.  When using this query parameter, the request body does not need to contain assets, but any assets in the request body will overwrite the copied assets.  #### Selection of _assets_ source  * If set as `<sourceName>[@<sourceVersionRange>]`, the _new function_ will be created with copied assets of the selected _source function_. * If set as `!example`, a `runtime` query parameter is required, and the _new function_ will be initialized with assets of the _runtime example_.  #### Selection of the _source function_  When `<sourceVersionRange>` is a range (or is not given), the latest _published_ version (in that range) is used.  If no _published_ version exists, the latest _draft_ is selected.  If no versions in the range exist, a `404` _Not Found_ error is returned.  #### The `name` of the _new function_  If a `name` is NOT specified (either as query parameter, or in an optional manifest asset in the request body), the `name` of the _new function_ will be that of the _source function_.  #### The `version` of the _new function_  When the _target_ and _source_ name are equal, the `version` query parameters is defaulted to `<sourceVersionRange>` (`~<sourceVersionRange>` when it's an exact version)  The version of the _new function_ will be: * If a `version` is NOT specified (either as query parameter, in an optional manifest asset, or as `<sourceVersionRange>` _default_)    * a **patch increment** (`<major>.<minor>.<patch>+1`) of the latest **existing version** with the target `name`    * **`1.0.0`** otherwise  * If a `version` is specified:    * the **lowest version** in that range **if no existing version** is in that range.    * an **increment** of the latest existing version, **at the highest level** (_major_,_minor_,_patch_) allowed by that range.    * otherwise, if all allowed versions already exist, a **`409` _Duplicate_ error** is raised.  #### Deployment overrides  The new function will use the deployment overrides of the copied function, unless a _manifest_ was specified in the request body.
         :type query['copy']: CreateWebscriptsCopyParameter
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -440,35 +431,39 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
+        if json is not None and should_validate:
             body_adapter = TypeAdapter(
                 Annotated[
                     Optional[Union[StrictBytes, StrictStr]],
                     Field(
                         description="The assets for a <em>plug</em> function can be provided as   <ul>     <li>A single <em>tar</em> archive (optionally compressed), with one of the content types      <code>application/octet-stream</code>, <code>application/tar</code>, <code>application/tar+gzip</code>, <code>application/x-gzip</code>, <code>application/x-tar</code>, <code>application/gzip</code></li>     <li>Separate files in a <code>multipart/form-data</code> request</li>     <li>A reference to the assets of another <em>plug</em> in the <code>copy</code> argument</li>   </ul>    The required <code>plug.json</code> json file contains the function metadata,   and must have a <code>runtime</code> attribute that is one of the supported <em>runtime</em>s    (see <code>GET /registry/v2/runtimes?functionType=plugs</code>).    For each <em>runtime</em> other files will be required or supported. "
                     ),
                 ]
             )
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
         body_args["content"] = content
         body_args["files"] = files
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(CreateQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": PostPlugJobSyncResponseV2 if not select_path else Model,
@@ -506,15 +501,14 @@
             ),
         ],
         *,
         query: DeleteAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostPlugJobSyncResponseV2 | PostPlugJobAsyncResponseV2: ...
 
     @overload
     async def delete_asset(
         self,
@@ -529,15 +523,14 @@
             ),
         ],
         *,
         query: DeleteAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def delete_asset(
         self,
@@ -552,15 +545,14 @@
             ),
         ],
         *,
         query: DeleteAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def delete_asset(
         self,
@@ -575,15 +567,14 @@
             ),
         ],
         *,
         query: DeleteAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def delete_asset(
         self,
@@ -598,15 +589,14 @@
             ),
         ],
         *,
         query: DeleteAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def delete_asset(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -620,46 +610,40 @@
             ),
         ],
         *,
         query: DeleteAssetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostPlugJobSyncResponseV2 | PostPlugJobAsyncResponseV2 | T | Response | Model:
         """Delete Plug Asset.
 
         Delete an asset from the plug's collection of existing assets.
         :param name: The name of the function. (required)
         :type name: str
         :param version: The version of the function. (required)
         :type version: str
         :param wildcard: Full path or path prefix of the asset within the archive (required)
         :type wildcard: str
         :param query: URL Query parameters.
         :type query: DeleteAssetQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['chown'] (dict) <br> query.chown (Query) : If set, ownership of the draft function is transferred to the current user.
         :type query['chown']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -670,26 +654,30 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
             "wildcard": str(wildcard),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(DeleteAssetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": PostPlugJobSyncResponseV2 if not select_path else Model,
@@ -723,15 +711,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> bytearray: ...
 
     @overload
     async def get_archive(
         self,
@@ -740,15 +727,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get_archive(
         self,
@@ -757,15 +743,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get_archive(
         self,
@@ -774,15 +759,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get_archive(
         self,
@@ -791,15 +775,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get_archive(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -807,15 +790,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetArchiveQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> bytearray | T | Response | Model:
         """Get Plug Archive.
 
         Get the specification archive of a plug.
         :param name: The name of the function. (required)
@@ -826,15 +808,14 @@
         :type query: GetArchiveQuery | QueryParamTypes, optional
         :param query['ls'] (dict) <br> query.ls (Query) : If set to `true`, the result will be a listing of the files in the asset, annotated with metadata and validation report from the asset conditions of the functions runtime.
         :type query['ls']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -845,25 +826,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetArchiveQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": bytearray if not select_path else Model,
@@ -900,15 +885,14 @@
             ),
         ],
         *,
         query: GetAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> bytearray: ...
 
     @overload
     async def get_asset(
         self,
@@ -923,15 +907,14 @@
             ),
         ],
         *,
         query: GetAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get_asset(
         self,
@@ -946,15 +929,14 @@
             ),
         ],
         *,
         query: GetAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get_asset(
         self,
@@ -969,15 +951,14 @@
             ),
         ],
         *,
         query: GetAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get_asset(
         self,
@@ -992,15 +973,14 @@
             ),
         ],
         *,
         query: GetAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get_asset(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -1014,15 +994,14 @@
             ),
         ],
         *,
         query: GetAssetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> bytearray | T | Response | Model:
         """Get File From Plug Archive.
 
         Get a file from the specification archive of a plug.
         :param name: The name of the function. (required)
@@ -1035,15 +1014,14 @@
         :type query: GetAssetQuery | QueryParamTypes, optional
         :param query['ls'] (dict) <br> query.ls (Query) : If set to `true`, the result will be a listing of the files in the asset, annotated with metadata and validation report from the asset conditions of the functions runtime.
         :type query['ls']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1054,26 +1032,30 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
             "wildcard": str(wildcard),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetAssetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": bytearray if not select_path else Model,
@@ -1101,84 +1083,78 @@
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetPlugResponseV2: ...
 
     @overload
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetPlugResponseV2 | T | Response | Model:
         """Get Latest Plug Version.
 
         Fetch the latest version of a <em>plug</em>.    By default, the result shows the latest non-deprecated, non-draft version.   If there is no such version, the latest deprecated or the latest draft version is returned, with the former taking precedence.       Use the boolean query parameters <code>includeDeprecated</code> or <code>includeDraft</code> to change this behaviour:   <ul>   <li><code>includeDeprecated=true</code>: do not prefer non-deprecated versions as a latest version: if the latest version is a deprecated one, it will be shown, even if there are older non-deprecated versions.</li>   <li><code>includeDraft=true</code>: do not prefer non-draft versions as a latest version: if the latest version is a draft, it will be shown, even if there are older non-draft versions.</li>   </ul>     The returned <em>plug version</em> will contain a link to its   latest _draft_ or latest _published_ version (if existing and different).
         :param name: The name of the function. (required)
@@ -1191,15 +1167,14 @@
         :type query['includeDraft']: bool
         :param query['includeDeprecated'] (dict) <br> query.include_deprecated (Query) : Configures the inclusion of _deprecated_ versions when selecting latest versions per name. By default, deprecated versions are only considered when no other versions are available. If set to `true`, deprecated versions are **included**. If set to `false`, deprecated versions are **excluded**.
         :type query['includeDeprecated']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1210,24 +1185,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetLatestQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": GetPlugResponseV2 if not select_path else Model,
@@ -1258,15 +1237,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetPlugResponseV2: ...
 
     @overload
     async def get(
         self,
@@ -1275,15 +1253,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get(
         self,
@@ -1292,15 +1269,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get(
         self,
@@ -1309,15 +1285,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get(
         self,
@@ -1326,15 +1301,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -1342,15 +1316,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetPlugResponseV2 | T | Response | Model:
         """Get Plug Version.
 
         Get a specific version of a plug.
         :param name: The name of the function. (required)
@@ -1359,15 +1332,14 @@
         :type version: str
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1378,25 +1350,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": GetPlugResponseV2 if not select_path else Model,
@@ -1427,15 +1403,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: JobsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> JobsForPlugResponseV2: ...
 
     @overload
     async def jobs(
         self,
@@ -1444,15 +1419,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: JobsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def jobs(
         self,
@@ -1461,15 +1435,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: JobsQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def jobs(
         self,
@@ -1478,15 +1451,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: JobsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def jobs(
         self,
@@ -1495,15 +1467,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: JobsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def jobs(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -1511,15 +1482,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: JobsQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> JobsForPlugResponseV2 | T | Response | Model:
         """List Plug Jobs.
 
         List the ongoing and completed operations on a specific plug.
         :param name: The name of the function. (required)
@@ -1540,15 +1510,14 @@
         :type query['createdBefore']: TimestampSpec
         :param query['createdAfter'] (dict) <br> query.created_after (Query) : Filter on jobs that created after the given timestamp or age
         :type query['createdAfter']: TimestampSpec
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1559,25 +1528,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(JobsQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": JobsForPlugResponseV2 if not select_path else Model,
@@ -1604,79 +1577,73 @@
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> LatestPlugsResponseV2: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> LatestPlugsResponseV2 | T | Response | Model:
         """List Plugs.
 
         List the (latest) versions of available <em>plugs</em>.  ### List Latest Plug Versions By default, the result includes the latest non-deprecated, non-draft version for each <em>plug</em> name. If there is no such version, the latest _deprecated_ or the latest _draft_ version is included, with the former taking precedence.     Use the boolean query parameters <code>includeDeprecated</code> or <code>includeDraft</code> to change this behaviour:   <ul>   <li><code>includeDeprecated=true</code>: do not prefer non-deprecated versions as a latest version: if the latest version is a deprecated one, it will be shown, even if there are older non-deprecated versions.</li>   <li><code>includeDraft=true</code>: do not prefer non-draft versions as a latest version: if the latest version is a draft, it will be shown, even if there are older non-draft versions.</li>   </ul>   As long as no version filters are used, each listed <em>plug version</em> contains representations of the latest draft (`entities[]._links.draft`)  or latest published (`entities[]._links.published`) version (if existing and different).   Use the query parameter `showRelated` to include only a link (default `showRelated=link`) or a full representation (`showRelated=embed`).  ### List Latest Plug Versions (with filter) When any of the _version filter_ query parameters are used, the response contains the _latest_ version per named <em>plug</em> that satisfy the filters, but **without links**.  ### List All Plug Versions When using `latest=false` (default when using the `namedVersion` filter), the listing contains _all_  <em>plugs</em> versions that satisfy the query, possibly multiple versions per named <em>plugs</em>. No HAL links are provided.  #### Filter on _status_ By default <em>plug versions</em> with status  `undeployed` are **excluded** in all cases. Use the _version filter_ `status` to include/exclude a status from the results. By example,  > `?status=any&includeDeprecated=true&includeDraft=true&latest=false`  will list _ALL_ versions known to the function registry.  #### Version filter parameters The following query parameters are _version filters_ for the <em>plug</em> listing: > `version`, `status`, `runtimeVersion`, `createdBy`, `createdBefore`, `createdAfter`, `updatedBy`, `updatedBefore`, `updatedAfter`, `nameVersion`, `deprecated`, `draft`, `tags`
         :param query: URL Query parameters.
@@ -1727,15 +1694,14 @@
         :type query['latest']: bool
         :param query['showRelated'] (dict) <br> query.show_related (Query) : Sets the representation of related function versions (like the _latest_ draft and/or published) in the response. - `embed`: as full summary representation (in `_embedded`). - `link`: as HAL link in (in `_links`). - `none`: omitted.
         :type query['showRelated']: ShowRelatedType
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1746,22 +1712,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(ListQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": LatestPlugsResponseV2 if not select_path else Model,
@@ -1789,84 +1759,78 @@
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PlugVersionsResponseV2: ...
 
     @overload
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PlugVersionsResponseV2 | T | Response | Model:
         """List Plug Versions.
 
         List all versions of a plug, including deprecated versions or not.
         :param name: The name of the function. (required)
@@ -1905,15 +1869,14 @@
         :type query['archiveFormat']: List[ArchiveFormat]
         :param query['runtime'] (dict) <br> query.runtime (Query) : Filter on the runtime of the function.
         :type query['runtime']: List[str]
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1924,24 +1887,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(ListVersionsQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": PlugVersionsResponseV2 if not select_path else Model,
@@ -1973,15 +1940,14 @@
         ],
         *,
         json: Documentation | None = None,
         query: PatchInterfaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetPlugResponseV2: ...
 
     @overload
     async def patch_interface(
         self,
@@ -1991,15 +1957,14 @@
         ],
         *,
         json: Documentation | None = None,
         query: PatchInterfaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def patch_interface(
         self,
@@ -2009,15 +1974,14 @@
         ],
         *,
         json: Documentation | None = None,
         query: PatchInterfaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def patch_interface(
         self,
@@ -2027,15 +1991,14 @@
         ],
         *,
         json: Documentation | None = None,
         query: PatchInterfaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def patch_interface(
         self,
@@ -2045,15 +2008,14 @@
         ],
         *,
         json: Documentation | None = None,
         query: PatchInterfaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def patch_interface(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -2062,15 +2024,14 @@
         ],
         *,
         json: Documentation | None = None,
         query: PatchInterfaceQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetPlugResponseV2 | T | Response | Model:
         """Patch Plug Interface.
 
         Patch the interface documentation of a plug version.
         :param name: The name of the function. (required)
@@ -2083,15 +2044,14 @@
         :type query: PatchInterfaceQuery | QueryParamTypes, optional
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -2102,29 +2062,33 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
+        if json is not None and should_validate:
             body_adapter = TypeAdapter(Optional[Documentation])
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(PatchInterfaceQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": GetPlugResponseV2 if not select_path else Model,
@@ -2156,15 +2120,14 @@
         ],
         *,
         json: UpdateMetadataRequestV2 | None = None,
         query: PatchMetadataQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetPlugResponseV2: ...
 
     @overload
     async def patch_metadata(
         self,
@@ -2174,15 +2137,14 @@
         ],
         *,
         json: UpdateMetadataRequestV2 | None = None,
         query: PatchMetadataQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def patch_metadata(
         self,
@@ -2192,15 +2154,14 @@
         ],
         *,
         json: UpdateMetadataRequestV2 | None = None,
         query: PatchMetadataQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def patch_metadata(
         self,
@@ -2210,15 +2171,14 @@
         ],
         *,
         json: UpdateMetadataRequestV2 | None = None,
         query: PatchMetadataQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def patch_metadata(
         self,
@@ -2228,15 +2188,14 @@
         ],
         *,
         json: UpdateMetadataRequestV2 | None = None,
         query: PatchMetadataQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def patch_metadata(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -2245,15 +2204,14 @@
         ],
         *,
         json: UpdateMetadataRequestV2 | None = None,
         query: PatchMetadataQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetPlugResponseV2 | T | Response | Model:
         """Patch Plug Metadata.
 
         Patch the metadata of a plug version.
         :param name: The name of the function. (required)
@@ -2266,15 +2224,14 @@
         :type query: PatchMetadataQuery | QueryParamTypes, optional
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -2285,29 +2242,33 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
+        if json is not None and should_validate:
             body_adapter = TypeAdapter(Optional[UpdateMetadataRequestV2])
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(PatchMetadataQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": GetPlugResponseV2 if not select_path else Model,
@@ -2338,15 +2299,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: PublishQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostPlugJobSyncResponseV2 | PostPlugJobAsyncResponseV2: ...
 
     @overload
     async def publish(
         self,
@@ -2355,15 +2315,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: PublishQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def publish(
         self,
@@ -2372,15 +2331,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: PublishQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def publish(
         self,
@@ -2389,15 +2347,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: PublishQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def publish(
         self,
@@ -2406,15 +2363,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: PublishQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def publish(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -2422,15 +2378,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: PublishQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostPlugJobSyncResponseV2 | PostPlugJobAsyncResponseV2 | T | Response | Model:
         """Publish Draft Plug.
 
         Mark the <em>plug</em> to be ready and stable, taking it out of draft mode.,    Typically, the <em>plug</em> should be in the <code>running</code> status,    such that publishing becomes a simple operation where the existing deployment can be re-used.   In other statuses, plug-registry may need to initiate a new build and deployment procedure.
         :param name: The name of the function. (required)
@@ -2449,15 +2404,14 @@
         :type query['deprecatePrevious']: DeprecatePreviousPolicy
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -2468,25 +2422,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(PublishQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": PostPlugJobSyncResponseV2 if not select_path else Model,
@@ -2518,15 +2476,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RebuildQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> RebuildPlugSyncResponseV2 | RebuildPlugAsyncResponseV2: ...
 
     @overload
     async def rebuild(
         self,
@@ -2535,15 +2492,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RebuildQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def rebuild(
         self,
@@ -2552,15 +2508,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RebuildQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def rebuild(
         self,
@@ -2569,15 +2524,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RebuildQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def rebuild(
         self,
@@ -2586,15 +2540,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RebuildQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def rebuild(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -2602,48 +2555,46 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RebuildQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> RebuildPlugSyncResponseV2 | RebuildPlugAsyncResponseV2 | T | Response | Model:
         """Rebuild Plug.
 
         Rebuild and deploy a plug with the original or updated base image.
         :param name: The name of the function. (required)
         :type name: str
         :param version: The version of the function. (required)
         :type version: str
         :param query: URL Query parameters.
         :type query: RebuildQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.
-        :type query['scaleToZero']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['dryRun'] (dict) <br> query.dry_run (Query) : If set to <code>true</code>, checks whether rebuild jobs are needed, but do not start any jobs.
         :type query['dryRun']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param query['upgrade'] (dict) <br> query.upgrade (Query) : If set, force a rebuild with the given <em>runtime</em> version selection policy. <ul>  <li><code>same</code> <b>patch</b> version.   This should only include backward compatible upgrades.  </li>  <li><code>minor</code> <b>major</b> version.   This might include an upgrade of e.g. the language runtime and/or provided   dependencies that could break compatiblity with the function. .</li> </ul>
         :type query['upgrade']: RebuildPolicy
         :param query['forceVersion'] (dict) <br> query.force_version (Query) : If set, force a rebuild with the given runtime version (including downgrades). This parameter is mutually exclusive to the `upgrade` parameter.
         :type query['forceVersion']: str
         :param query['ignoreChecks'] (dict) <br> query.ignore_checks (Query) : If set to true, checks that normally prevent a rebuild are overriden. These checks include: * function state in `pending`, `running`, `failed` or `undeployed` * backoff period due to recent failures * usage of deprecated dependencies * running jobs on entity * the `dryRun` option
         :type query['ignoreChecks']: bool
+        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful (re-)deployment. If not set, the function is scaled to zero only if it was not active before this command.
+        :type query['scaleToZero']: bool
         :param query['skipRebuild'] (dict) <br> query.skip_rebuild (Query) : If set, the function will not be rebuild. Always uses the current runtime version when re-deploying/re-verifying the function.
         :type query['skipRebuild']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -2654,25 +2605,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(RebuildQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": RebuildPlugSyncResponseV2 if not select_path else Model,
@@ -2704,15 +2659,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RemoveVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> UndeployedResponseV2 | UndeploySubmittedResponseV2: ...
 
     @overload
     async def remove_version(
         self,
@@ -2721,15 +2675,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RemoveVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def remove_version(
         self,
@@ -2738,15 +2691,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RemoveVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def remove_version(
         self,
@@ -2755,15 +2707,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RemoveVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def remove_version(
         self,
@@ -2772,15 +2723,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RemoveVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def remove_version(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -2788,15 +2738,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RemoveVersionQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> UndeployedResponseV2 | UndeploySubmittedResponseV2 | T | Response | Model:
         """Remove Plug Version.
 
         Deprecate, undeploy and/or remove a <em>plug</em> version.  By default, a `DELETE`  * marks _published_ version(s) _deprecated_: they remain active, but are no longer included in listings by default. * completely removes any _draft_ version(s) (_deprecate_, _undeploy_ and _remove_)  A _deprecated_ plug version will eventually be _undeployed_ (but not _removed_) by an external background task,  once proven that no waylay rule template or task references it.  Use `?force=true` to skip the deprecation and immediately remove the version(s).  Use `?undeploy=true` to undeploy the plug version(s), but keep it registered in a `undeployed` state. An `undeployed` version can later be restored by a _rebuild_ action.
         :param name: The name of the function. (required)
@@ -2813,15 +2762,14 @@
         :type query['force']: bool
         :param query['undeploy'] (dict) <br> query.undeploy (Query) : If `true`, the `DELETE` operation * undeploys the (openfaas) function for the plug: it becomes no longer available for invocation. * does NOT remove the plug from registry: it stays in an `undeployed` status.  All assets and definitions are retained, so the plug can be restored later with a  _rebuild_ action.  If `false`, the `DELETE` operation * _only_ marks the plug version(s) as _deprecated_: the plug remains active but is removed from the default listings.   This also applies to _draft_ versions.  This parameter is incompatible with `force=true`.  If not set the default behaviour applies: * _draft_ versions are _undeployed_ and _removed_ from registry. * non-_draft_ versions are marked _deprecated_ only.
         :type query['undeploy']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -2832,25 +2780,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(RemoveVersionQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": UndeployedResponseV2 if not select_path else Model,
@@ -2879,84 +2831,78 @@
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: RemoveVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> UndeployedResponseV2 | UndeploySubmittedResponseV2: ...
 
     @overload
     async def remove_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: RemoveVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def remove_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: RemoveVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def remove_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: RemoveVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def remove_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: RemoveVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def remove_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: RemoveVersionsQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> UndeployedResponseV2 | UndeploySubmittedResponseV2 | T | Response | Model:
         """Remove Plug.
 
         Deprecate, undeploy and/or remove all versions of this named <em>plug</em>.  By default, a `DELETE`  * marks _published_ version(s) _deprecated_: they remain active, but are no longer included in listings by default. * completely removes any _draft_ version(s) (_deprecate_, _undeploy_ and _remove_)  A _deprecated_ plug version will eventually be _undeployed_ (but not _removed_) by an external background task,  once proven that no waylay rule template or task references it.  Use `?force=true` to skip the deprecation and immediately remove the version(s).  Use `?undeploy=true` to undeploy the plug version(s), but keep it registered in a `undeployed` state. An `undeployed` version can later be restored by a _rebuild_ action.
         :param name: The name of the function. (required)
@@ -2971,15 +2917,14 @@
         :type query['force']: bool
         :param query['undeploy'] (dict) <br> query.undeploy (Query) : If `true`, the `DELETE` operation * undeploys the (openfaas) function for the plug: it becomes no longer available for invocation. * does NOT remove the plug from registry: it stays in an `undeployed` status.  All assets and definitions are retained, so the plug can be restored later with a  _rebuild_ action.  If `false`, the `DELETE` operation * _only_ marks the plug version(s) as _deprecated_: the plug remains active but is removed from the default listings.   This also applies to _draft_ versions.  This parameter is incompatible with `force=true`.  If not set the default behaviour applies: * _draft_ versions are _undeployed_ and _removed_ from registry. * non-_draft_ versions are marked _deprecated_ only.
         :type query['undeploy']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -2990,24 +2935,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(RemoveVersionsQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": UndeployedResponseV2 if not select_path else Model,
@@ -3048,15 +2997,14 @@
         content: Annotated[
             RequestContent | None, Field(description="A single asset file.")
         ] = None,
         query: UpdateAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostPlugJobSyncResponseV2 | PostPlugJobAsyncResponseV2: ...
 
     @overload
     async def update_asset(
         self,
@@ -3074,15 +3022,14 @@
         content: Annotated[
             RequestContent | None, Field(description="A single asset file.")
         ] = None,
         query: UpdateAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def update_asset(
         self,
@@ -3100,15 +3047,14 @@
         content: Annotated[
             RequestContent | None, Field(description="A single asset file.")
         ] = None,
         query: UpdateAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def update_asset(
         self,
@@ -3126,15 +3072,14 @@
         content: Annotated[
             RequestContent | None, Field(description="A single asset file.")
         ] = None,
         query: UpdateAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def update_asset(
         self,
@@ -3152,15 +3097,14 @@
         content: Annotated[
             RequestContent | None, Field(description="A single asset file.")
         ] = None,
         query: UpdateAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def update_asset(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -3177,15 +3121,14 @@
         content: Annotated[
             RequestContent | None, Field(description="A single asset file.")
         ] = None,
         query: UpdateAssetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostPlugJobSyncResponseV2 | PostPlugJobAsyncResponseV2 | T | Response | Model:
         """Update Plug Asset.
 
         The provided asset will be added to the <em>plug</em> function's collection of existing assets,   replacing any existing asset with the same name.    Please note that it is not allowed to update the plug.json json file with a changed value for any of the     <code>name</code>, <code>version</code> and/or <code>runtime</code> attributes.    For each <em>runtime</em> other files are supported.
         :param name: The name of the function. (required)
@@ -3194,31 +3137,26 @@
         :type version: str
         :param wildcard: Full path or path prefix of the asset within the archive (required)
         :type wildcard: str
         :param content: A single asset file.
         :type content: ContentRequest, optional
         :param query: URL Query parameters.
         :type query: UpdateAssetQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['chown'] (dict) <br> query.chown (Query) : If set, ownership of the draft function is transferred to the current user.
         :type query['chown']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -3229,27 +3167,31 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
             "wildcard": str(wildcard),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
         body_args["content"] = content
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(UpdateAssetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": PostPlugJobSyncResponseV2 if not select_path else Model,
@@ -3292,15 +3234,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: UpdateAssetsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostPlugJobSyncResponseV2 | PostPlugJobAsyncResponseV2: ...
 
     @overload
     async def update_assets(
         self,
@@ -3318,15 +3259,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: UpdateAssetsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def update_assets(
         self,
@@ -3344,15 +3284,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: UpdateAssetsQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def update_assets(
         self,
@@ -3370,15 +3309,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: UpdateAssetsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def update_assets(
         self,
@@ -3396,15 +3334,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: UpdateAssetsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def update_assets(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -3421,15 +3358,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: UpdateAssetsQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostPlugJobSyncResponseV2 | PostPlugJobAsyncResponseV2 | T | Response | Model:
         """Update Plug Assets.
 
         Update a draft <em>plug</em> function by updating its assets.      The assets for a <em>plug</em> function can be provided as either   <ul>     <li>a single <em>tar</em> archive (optionally compressed), with one of the content types      <code>application/octet-stream</code>, <code>application/tar</code>, <code>application/tar+gzip</code>, <code>application/x-gzip</code>, <code>application/x-tar</code>, <code>application/gzip</code></li>     <li>separate files in a <code>multipart/form-data</code> request</li>   </ul>    The provided assets will be added to the <em>plug</em> function's collection of existing assets,   replacing any existing assets with the same name.    Please note that it is not allowed to update the plug.json</code> json file with a changed value for any of the    <code>name</code>, <code>version</code> and/or <code>runtime</code> attributes.    For each <em>runtime</em> other files are supported.
         :param name: The name of the function. (required)
@@ -3438,31 +3374,26 @@
         :type version: str
         :param content: The assets for a <em>plug</em> function can be provided as either   <ul>     <li>a single <em>tar</em> archive (optionally compressed), with one of the content types      <code>application/octet-stream</code>, <code>application/tar</code>, <code>application/tar+gzip</code>, <code>application/x-gzip</code>, <code>application/x-tar</code>, <code>application/gzip</code></li>     <li>separate files in a <code>multipart/form-data</code> request</li>   </ul>    The provided assets will be added to the <em>plug</em> function's collection of existing assets,   replacing any existing assets with the same name.    Please note that it is not allowed to update the plug.json</code> json file with a changed value for any of the    <code>name</code>, <code>version</code> and/or <code>runtime</code> attributes.    For each <em>runtime</em> other files are supported.
         :type content: ContentRequest, optional
         :param files: The files of a `content-type: multipart/form-data` request.
         :type files: FilesRequest, optional
         :param query: URL Query parameters.
         :type query: UpdateAssetsQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['chown'] (dict) <br> query.chown (Query) : If set, ownership of the draft function is transferred to the current user.
         :type query['chown']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -3473,27 +3404,31 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
         body_args["content"] = content
         body_args["files"] = files
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(UpdateAssetsQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": PostPlugJobSyncResponseV2 if not select_path else Model,
@@ -3527,15 +3462,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: VerifyQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> VerifyPlugSyncResponseV2 | PostPlugJobAsyncResponseV2: ...
 
     @overload
     async def verify(
         self,
@@ -3544,15 +3478,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: VerifyQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def verify(
         self,
@@ -3561,15 +3494,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: VerifyQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def verify(
         self,
@@ -3578,15 +3510,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: VerifyQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def verify(
         self,
@@ -3595,15 +3526,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: VerifyQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def verify(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -3611,36 +3541,34 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: VerifyQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> VerifyPlugSyncResponseV2 | PostPlugJobAsyncResponseV2 | T | Response | Model:
         """Verify Health Of Plug.
 
         Verify health of plug deployed on openfaas.
         :param name: The name of the function. (required)
         :type name: str
         :param version: The version of the function. (required)
         :type version: str
         :param query: URL Query parameters.
         :type query: VerifyQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.
-        :type query['scaleToZero']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
+        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.
+        :type query['scaleToZero']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -3651,25 +3579,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(VerifyQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": VerifyPlugSyncResponseV2 if not select_path else Model,
```

### Comparing `waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/api/runtimes_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/runtimes_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -112,15 +112,14 @@
             Any, Field(description="A version range for a <em>runtime</em>")
         ],
         *,
         query: ExampleArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> bytearray: ...
 
     @overload
     async def example_archive(
         self,
@@ -129,15 +128,14 @@
             Any, Field(description="A version range for a <em>runtime</em>")
         ],
         *,
         query: ExampleArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def example_archive(
         self,
@@ -146,15 +144,14 @@
             Any, Field(description="A version range for a <em>runtime</em>")
         ],
         *,
         query: ExampleArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def example_archive(
         self,
@@ -163,15 +160,14 @@
             Any, Field(description="A version range for a <em>runtime</em>")
         ],
         *,
         query: ExampleArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def example_archive(
         self,
@@ -180,15 +176,14 @@
             Any, Field(description="A version range for a <em>runtime</em>")
         ],
         *,
         query: ExampleArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def example_archive(
         self,
         name: Annotated[StrictStr, Field(description="The name of a <em>runtime</em>")],
@@ -196,15 +191,14 @@
             Any, Field(description="A version range for a <em>runtime</em>")
         ],
         *,
         query: ExampleArchiveQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> bytearray | T | Response | Model:
         """Get Runtime Example Archive.
 
         Get an example of the specification archive of the runtime.
         :param name: The name of a <em>runtime</em> (required)
@@ -217,15 +211,14 @@
         :type query['ls']: bool
         :param query['includeDeprecated'] (dict) <br> query.include_deprecated (Query) : If set to `true`, deprecated runtimes will be included in the query.
         :type query['includeDeprecated']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -236,25 +229,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(ExampleArchiveQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": bytearray if not select_path else Model,
@@ -291,15 +288,14 @@
             ),
         ],
         *,
         query: GetExampleAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> bytearray: ...
 
     @overload
     async def get_example_asset(
         self,
@@ -314,15 +310,14 @@
             ),
         ],
         *,
         query: GetExampleAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get_example_asset(
         self,
@@ -337,15 +332,14 @@
             ),
         ],
         *,
         query: GetExampleAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get_example_asset(
         self,
@@ -360,15 +354,14 @@
             ),
         ],
         *,
         query: GetExampleAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get_example_asset(
         self,
@@ -383,15 +376,14 @@
             ),
         ],
         *,
         query: GetExampleAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get_example_asset(
         self,
         name: Annotated[StrictStr, Field(description="The name of a <em>runtime</em>")],
@@ -405,15 +397,14 @@
             ),
         ],
         *,
         query: GetExampleAssetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> bytearray | T | Response | Model:
         """Get File From Runtime Example Archive.
 
         Get a file from the example specification archive of the runtime.
         :param name: The name of a <em>runtime</em> (required)
@@ -428,15 +419,14 @@
         :type query['ls']: bool
         :param query['includeDeprecated'] (dict) <br> query.include_deprecated (Query) : If set to `true`, deprecated runtimes will be included in the query.
         :type query['includeDeprecated']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -447,26 +437,30 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
             "wildcard": str(wildcard),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetExampleAssetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": bytearray if not select_path else Model,
@@ -494,84 +488,78 @@
         self,
         name: Annotated[StrictStr, Field(description="The name of a <em>runtime</em>")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> RuntimeVersionResponse: ...
 
     @overload
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of a <em>runtime</em>")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of a <em>runtime</em>")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of a <em>runtime</em>")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of a <em>runtime</em>")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of a <em>runtime</em>")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> RuntimeVersionResponse | T | Response | Model:
         """Get Latest Runtime Version.
 
         Get a representation of the default runtime version by name.
         :param name: The name of a <em>runtime</em> (required)
@@ -586,15 +574,14 @@
         :type query['functionType']: List[FunctionType]
         :param query['archiveFormat'] (dict) <br> query.archive_format (Query) : If set, filters on the <code>archiveFormat</code> of a runtime. Uses an exact match.
         :type query['archiveFormat']: List[ArchiveFormat]
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -605,24 +592,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetLatestQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": RuntimeVersionResponse if not select_path else Model,
@@ -653,15 +644,14 @@
             Any, Field(description="A version range for a <em>runtime</em>")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> RuntimeVersionResponse: ...
 
     @overload
     async def get(
         self,
@@ -670,15 +660,14 @@
             Any, Field(description="A version range for a <em>runtime</em>")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get(
         self,
@@ -687,15 +676,14 @@
             Any, Field(description="A version range for a <em>runtime</em>")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get(
         self,
@@ -704,15 +692,14 @@
             Any, Field(description="A version range for a <em>runtime</em>")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get(
         self,
@@ -721,15 +708,14 @@
             Any, Field(description="A version range for a <em>runtime</em>")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get(
         self,
         name: Annotated[StrictStr, Field(description="The name of a <em>runtime</em>")],
@@ -737,15 +723,14 @@
             Any, Field(description="A version range for a <em>runtime</em>")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> RuntimeVersionResponse | T | Response | Model:
         """Get Runtime Version.
 
         Get a representation of the default runtime version by name.
         :param name: The name of a <em>runtime</em> (required)
@@ -756,15 +741,14 @@
         :type query: GetQuery | QueryParamTypes, optional
         :param query['includeDeprecated'] (dict) <br> query.include_deprecated (Query) : If set to `true`, deprecated runtimes will be included in the query.
         :type query['includeDeprecated']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -775,25 +759,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": RuntimeVersionResponse if not select_path else Model,
@@ -820,79 +808,73 @@
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> RuntimeSummaryResponse: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> RuntimeSummaryResponse | T | Response | Model:
         """List Runtimes.
 
         List the runtimes that function registry supports.
         :param query: URL Query parameters.
@@ -909,15 +891,14 @@
         :type query['functionType']: List[FunctionType]
         :param query['archiveFormat'] (dict) <br> query.archive_format (Query) : If set, filters on the <code>archiveFormat</code> of a runtime. Uses an exact match.
         :type query['archiveFormat']: List[ArchiveFormat]
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -928,22 +909,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(ListQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": RuntimeSummaryResponse if not select_path else Model,
@@ -971,84 +956,78 @@
         self,
         name: Annotated[StrictStr, Field(description="The name of a <em>runtime</em>")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> RuntimeSummaryResponse: ...
 
     @overload
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of a <em>runtime</em>")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of a <em>runtime</em>")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of a <em>runtime</em>")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of a <em>runtime</em>")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of a <em>runtime</em>")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> RuntimeSummaryResponse | T | Response | Model:
         """List Runtime Versions.
 
         List the supported versions of a specific runtime.
         :param name: The name of a <em>runtime</em> (required)
@@ -1065,15 +1044,14 @@
         :type query['functionType']: List[FunctionType]
         :param query['archiveFormat'] (dict) <br> query.archive_format (Query) : If set, filters on the <code>archiveFormat</code> of a runtime. Uses an exact match.
         :type query['archiveFormat']: List[ArchiveFormat]
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1084,24 +1062,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(ListVersionsQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": RuntimeSummaryResponse if not select_path else Model,
```

### Comparing `waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/api/schemas_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/schemas_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,89 +76,83 @@
         function_type: Annotated[FunctionType, Field(description="Function type")],
         role: Annotated[AssetRole, Field(description="Asset role")],
         *,
         query: GetByRoleQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Dict[str, object]: ...
 
     @overload
     async def get_by_role(
         self,
         function_type: Annotated[FunctionType, Field(description="Function type")],
         role: Annotated[AssetRole, Field(description="Asset role")],
         *,
         query: GetByRoleQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get_by_role(
         self,
         function_type: Annotated[FunctionType, Field(description="Function type")],
         role: Annotated[AssetRole, Field(description="Asset role")],
         *,
         query: GetByRoleQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get_by_role(
         self,
         function_type: Annotated[FunctionType, Field(description="Function type")],
         role: Annotated[AssetRole, Field(description="Asset role")],
         *,
         query: GetByRoleQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get_by_role(
         self,
         function_type: Annotated[FunctionType, Field(description="Function type")],
         role: Annotated[AssetRole, Field(description="Asset role")],
         *,
         query: GetByRoleQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get_by_role(
         self,
         function_type: Annotated[FunctionType, Field(description="Function type")],
         role: Annotated[AssetRole, Field(description="Asset role")],
         *,
         query: GetByRoleQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Dict[str, object] | T | Response | Model:
         """Get Asset Schema (Deprecated).
 
         Get the JSON schema that is used to validate the asset.
         :param function_type: Function type (required)
@@ -167,15 +161,14 @@
         :type role: AssetRole
         :param query: URL Query parameters.
         :type query: GetByRoleQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -190,26 +183,29 @@
             object wraps both the http Response and any parsed data.
         """
 
         warnings.warn(
             "GET /registry/v2/schemas/{functionType}/{role}/schema is deprecated.",
             DeprecationWarning,
         )
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
 
         # path parameters
         path_params: Dict[str, str] = {
             "functionType": str(function_type),
             "role": str(role),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetByRoleQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": Dict[str, object] if not select_path else Model,
@@ -237,99 +233,92 @@
         self,
         schema_id: Annotated[StrictStr, Field(description="Schema id")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Dict[str, object]: ...
 
     @overload
     async def get(
         self,
         schema_id: Annotated[StrictStr, Field(description="Schema id")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get(
         self,
         schema_id: Annotated[StrictStr, Field(description="Schema id")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get(
         self,
         schema_id: Annotated[StrictStr, Field(description="Schema id")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get(
         self,
         schema_id: Annotated[StrictStr, Field(description="Schema id")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get(
         self,
         schema_id: Annotated[StrictStr, Field(description="Schema id")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Dict[str, object] | T | Response | Model:
         """Get Asset Schema.
 
         Get the JSON schema that is used to validate an asset.
         :param schema_id: Schema id (required)
         :type schema_id: str
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -340,24 +329,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "schemaId": str(schema_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": Dict[str, object] if not select_path else Model,
```

### Comparing `waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/api/webscripts_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/webscripts_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -230,15 +230,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostWebscriptJobSyncResponseV2 | PostWebscriptJobAsyncResponseV2: ...
 
     @overload
     async def create(
         self,
@@ -258,15 +257,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def create(
         self,
@@ -286,15 +284,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def create(
         self,
@@ -314,15 +311,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def create(
         self,
@@ -342,15 +338,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def create(
         self,
         *,
@@ -369,15 +364,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> (
         PostWebscriptJobSyncResponseV2
         | PostWebscriptJobAsyncResponseV2
         | T
         | Response
@@ -390,43 +384,40 @@
         :type json: bytearray, optional
         :param content: The assets for a <em>webscript</em> function can be provided as   <ul>     <li>A single <em>tar</em> archive (optionally compressed), with one of the content types      <code>application/octet-stream</code>, <code>application/tar</code>, <code>application/tar+gzip</code>, <code>application/x-gzip</code>, <code>application/x-tar</code>, <code>application/gzip</code></li>     <li>Separate files in a <code>multipart/form-data</code> request</li>     <li>A reference to the assets of another <em>webscript</em> in the <code>copy</code> argument</li>   </ul>    The required <code>webscript.json</code> json file contains the function metadata,   and must have a <code>runtime</code> attribute that is one of the supported <em>runtime</em>s    (see <code>GET /registry/v2/runtimes?functionType=webscripts</code>).    For each <em>runtime</em> other files will be required or supported.
         :type content: ContentRequest, optional
         :param files: The files of a `content-type: multipart/form-data` request.
         :type files: FilesRequest, optional
         :param query: URL Query parameters.
         :type query: CreateQuery | QueryParamTypes, optional
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
         :param query['deprecatePrevious'] (dict) <br> query.deprecate_previous (Query) : Set the cleanup policy used to automatically deprecate/delete previous versions.
         :type query['deprecatePrevious']: DeprecatePreviousPolicy
         :param query['dryRun'] (dict) <br> query.dry_run (Query) : If set to <code>true</code>, validates the deployment conditions, but does not change anything.
         :type query['dryRun']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
+        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. Saves computing resources when the function is not to be used immediately.
+        :type query['scaleToZero']: bool
         :param query['version'] (dict) <br> query.version (Query) : If set, the function version will be an increment of the latest existing version that satisfies the `version` range. Note that this increment always takes precedence over an explicit `version` in the function manifest.
         :type query['version']: SemanticVersionRange
         :param query['name'] (dict) <br> query.name (Query) : If set, the value will be used as the function name instead of the one specified in the manifest.
         :type query['name']: str
         :param query['draft'] (dict) <br> query.draft (Query) : If set, the created function will be a draft function and its assets are still mutable. A build and deploy is initiated only in the case when all necessary assets are present and valid.
         :type query['draft']: bool
         :param query['runtime'] (dict) <br> query.runtime (Query) : If set, the created function will use the indicated runtime (latest version within specified range).  This takes precedence over the runtime specified in a function manifest (copied or from request body).
         :type query['runtime']: str
         :param query['copy'] (dict) <br> query.copy_from (Query) : Indicates the _source_ of initial assets for a _new function_.  When using this query parameter, the request body does not need to contain assets, but any assets in the request body will overwrite the copied assets.  #### Selection of _assets_ source  * If set as `<sourceName>[@<sourceVersionRange>]`, the _new function_ will be created with copied assets of the selected _source function_. * If set as `!example`, a `runtime` query parameter is required, and the _new function_ will be initialized with assets of the _runtime example_.  #### Selection of the _source function_  When `<sourceVersionRange>` is a range (or is not given), the latest _published_ version (in that range) is used.  If no _published_ version exists, the latest _draft_ is selected.  If no versions in the range exist, a `404` _Not Found_ error is returned.  #### The `name` of the _new function_  If a `name` is NOT specified (either as query parameter, or in an optional manifest asset in the request body), the `name` of the _new function_ will be that of the _source function_.  #### The `version` of the _new function_  When the _target_ and _source_ name are equal, the `version` query parameters is defaulted to `<sourceVersionRange>` (`~<sourceVersionRange>` when it's an exact version)  The version of the _new function_ will be: * If a `version` is NOT specified (either as query parameter, in an optional manifest asset, or as `<sourceVersionRange>` _default_)    * a **patch increment** (`<major>.<minor>.<patch>+1`) of the latest **existing version** with the target `name`    * **`1.0.0`** otherwise  * If a `version` is specified:    * the **lowest version** in that range **if no existing version** is in that range.    * an **increment** of the latest existing version, **at the highest level** (_major_,_minor_,_patch_) allowed by that range.    * otherwise, if all allowed versions already exist, a **`409` _Duplicate_ error** is raised.  #### Deployment overrides  The new function will use the deployment overrides of the copied function, unless a _manifest_ was specified in the request body.
         :type query['copy']: CreateWebscriptsCopyParameter
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -437,35 +428,39 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
+        if json is not None and should_validate:
             body_adapter = TypeAdapter(
                 Annotated[
                     Optional[Union[StrictBytes, StrictStr]],
                     Field(
                         description="The assets for a <em>webscript</em> function can be provided as   <ul>     <li>A single <em>tar</em> archive (optionally compressed), with one of the content types      <code>application/octet-stream</code>, <code>application/tar</code>, <code>application/tar+gzip</code>, <code>application/x-gzip</code>, <code>application/x-tar</code>, <code>application/gzip</code></li>     <li>Separate files in a <code>multipart/form-data</code> request</li>     <li>A reference to the assets of another <em>webscript</em> in the <code>copy</code> argument</li>   </ul>    The required <code>webscript.json</code> json file contains the function metadata,   and must have a <code>runtime</code> attribute that is one of the supported <em>runtime</em>s    (see <code>GET /registry/v2/runtimes?functionType=webscripts</code>).    For each <em>runtime</em> other files will be required or supported. "
                     ),
                 ]
             )
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
         body_args["content"] = content
         body_args["files"] = files
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(CreateQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": PostWebscriptJobSyncResponseV2 if not select_path else Model,
@@ -503,15 +498,14 @@
             ),
         ],
         *,
         query: DeleteAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostWebscriptJobSyncResponseV2 | PostWebscriptJobAsyncResponseV2: ...
 
     @overload
     async def delete_asset(
         self,
@@ -526,15 +520,14 @@
             ),
         ],
         *,
         query: DeleteAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def delete_asset(
         self,
@@ -549,15 +542,14 @@
             ),
         ],
         *,
         query: DeleteAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def delete_asset(
         self,
@@ -572,15 +564,14 @@
             ),
         ],
         *,
         query: DeleteAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def delete_asset(
         self,
@@ -595,15 +586,14 @@
             ),
         ],
         *,
         query: DeleteAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def delete_asset(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -617,15 +607,14 @@
             ),
         ],
         *,
         query: DeleteAssetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> (
         PostWebscriptJobSyncResponseV2
         | PostWebscriptJobAsyncResponseV2
         | T
         | Response
@@ -638,31 +627,26 @@
         :type name: str
         :param version: The version of the function. (required)
         :type version: str
         :param wildcard: Full path or path prefix of the asset within the archive (required)
         :type wildcard: str
         :param query: URL Query parameters.
         :type query: DeleteAssetQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['chown'] (dict) <br> query.chown (Query) : If set, ownership of the draft function is transferred to the current user.
         :type query['chown']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -673,26 +657,30 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
             "wildcard": str(wildcard),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(DeleteAssetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": PostWebscriptJobSyncResponseV2 if not select_path else Model,
@@ -726,15 +714,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> bytearray: ...
 
     @overload
     async def get_archive(
         self,
@@ -743,15 +730,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get_archive(
         self,
@@ -760,15 +746,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get_archive(
         self,
@@ -777,15 +762,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get_archive(
         self,
@@ -794,15 +778,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetArchiveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get_archive(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -810,15 +793,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetArchiveQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> bytearray | T | Response | Model:
         """Get Webscript Archive.
 
         Get the specification archive of a webscript.
         :param name: The name of the function. (required)
@@ -829,15 +811,14 @@
         :type query: GetArchiveQuery | QueryParamTypes, optional
         :param query['ls'] (dict) <br> query.ls (Query) : If set to `true`, the result will be a listing of the files in the asset, annotated with metadata and validation report from the asset conditions of the functions runtime.
         :type query['ls']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -848,25 +829,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetArchiveQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": bytearray if not select_path else Model,
@@ -903,15 +888,14 @@
             ),
         ],
         *,
         query: GetAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> bytearray: ...
 
     @overload
     async def get_asset(
         self,
@@ -926,15 +910,14 @@
             ),
         ],
         *,
         query: GetAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get_asset(
         self,
@@ -949,15 +932,14 @@
             ),
         ],
         *,
         query: GetAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get_asset(
         self,
@@ -972,15 +954,14 @@
             ),
         ],
         *,
         query: GetAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get_asset(
         self,
@@ -995,15 +976,14 @@
             ),
         ],
         *,
         query: GetAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get_asset(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -1017,15 +997,14 @@
             ),
         ],
         *,
         query: GetAssetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> bytearray | T | Response | Model:
         """Get File From Webscript Archive.
 
         Get a file from the specification archive of a webscript.
         :param name: The name of the function. (required)
@@ -1038,15 +1017,14 @@
         :type query: GetAssetQuery | QueryParamTypes, optional
         :param query['ls'] (dict) <br> query.ls (Query) : If set to `true`, the result will be a listing of the files in the asset, annotated with metadata and validation report from the asset conditions of the functions runtime.
         :type query['ls']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1057,26 +1035,30 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
             "wildcard": str(wildcard),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetAssetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": bytearray if not select_path else Model,
@@ -1104,84 +1086,78 @@
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetWebscriptResponseV2: ...
 
     @overload
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get_latest(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: GetLatestQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetWebscriptResponseV2 | T | Response | Model:
         """Get Latest Webscript Version.
 
         Fetch the latest version of a <em>webscript</em>.    By default, the result shows the latest non-deprecated, non-draft version.   If there is no such version, the latest deprecated or the latest draft version is returned, with the former taking precedence.       Use the boolean query parameters <code>includeDeprecated</code> or <code>includeDraft</code> to change this behaviour:   <ul>   <li><code>includeDeprecated=true</code>: do not prefer non-deprecated versions as a latest version: if the latest version is a deprecated one, it will be shown, even if there are older non-deprecated versions.</li>   <li><code>includeDraft=true</code>: do not prefer non-draft versions as a latest version: if the latest version is a draft, it will be shown, even if there are older non-draft versions.</li>   </ul>     The returned <em>webscript version</em> will contain a link to its   latest _draft_ or latest _published_ version (if existing and different).
         :param name: The name of the function. (required)
@@ -1192,15 +1168,14 @@
         :type query['includeDraft']: bool
         :param query['includeDeprecated'] (dict) <br> query.include_deprecated (Query) : Configures the inclusion of _deprecated_ versions when selecting latest versions per name. By default, deprecated versions are only considered when no other versions are available. If set to `true`, deprecated versions are **included**. If set to `false`, deprecated versions are **excluded**.
         :type query['includeDeprecated']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1211,24 +1186,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetLatestQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": GetWebscriptResponseV2 if not select_path else Model,
@@ -1259,15 +1238,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetWebscriptResponseV2: ...
 
     @overload
     async def get(
         self,
@@ -1276,15 +1254,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get(
         self,
@@ -1293,15 +1270,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get(
         self,
@@ -1310,15 +1286,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get(
         self,
@@ -1327,15 +1302,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -1343,15 +1317,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetWebscriptResponseV2 | T | Response | Model:
         """Get Webscript Version.
 
         Get the webscript version.
         :param name: The name of the function. (required)
@@ -1360,15 +1333,14 @@
         :type version: str
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1379,25 +1351,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": GetWebscriptResponseV2 if not select_path else Model,
@@ -1428,15 +1404,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: JobsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> JobsForWebscriptResponseV2: ...
 
     @overload
     async def jobs(
         self,
@@ -1445,15 +1420,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: JobsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def jobs(
         self,
@@ -1462,15 +1436,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: JobsQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def jobs(
         self,
@@ -1479,15 +1452,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: JobsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def jobs(
         self,
@@ -1496,15 +1468,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: JobsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def jobs(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -1512,15 +1483,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: JobsQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> JobsForWebscriptResponseV2 | T | Response | Model:
         """List Webscript Jobs.
 
         List the ongoing and completed operations on a specific webscript.
         :param name: The name of the function. (required)
@@ -1541,15 +1511,14 @@
         :type query['createdBefore']: TimestampSpec
         :param query['createdAfter'] (dict) <br> query.created_after (Query) : Filter on jobs that created after the given timestamp or age
         :type query['createdAfter']: TimestampSpec
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1560,25 +1529,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(JobsQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": JobsForWebscriptResponseV2 if not select_path else Model,
@@ -1606,84 +1579,78 @@
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> WebscriptVersionsResponseV2: ...
 
     @overload
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: ListVersionsQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> WebscriptVersionsResponseV2 | T | Response | Model:
         """List Webscript Versions.
 
         List all deployed versions of a webscript.
         :param name: The name of the function. (required)
@@ -1720,15 +1687,14 @@
         :type query['archiveFormat']: List[ArchiveFormat]
         :param query['runtime'] (dict) <br> query.runtime (Query) : Filter on the runtime of the function.
         :type query['runtime']: List[str]
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1739,24 +1705,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(ListVersionsQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": WebscriptVersionsResponseV2 if not select_path else Model,
@@ -1783,79 +1753,73 @@
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> LatestWebscriptsResponseV2: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> LatestWebscriptsResponseV2 | T | Response | Model:
         """List Webscripts.
 
         List the (latest) versions of available <em>webscripts</em>.  ### List Latest Webscript Versions By default, the result includes the latest non-deprecated, non-draft version for each <em>webscript</em> name. If there is no such version, the latest _deprecated_ or the latest _draft_ version is included, with the former taking precedence.     Use the boolean query parameters <code>includeDeprecated</code> or <code>includeDraft</code> to change this behaviour:   <ul>   <li><code>includeDeprecated=true</code>: do not prefer non-deprecated versions as a latest version: if the latest version is a deprecated one, it will be shown, even if there are older non-deprecated versions.</li>   <li><code>includeDraft=true</code>: do not prefer non-draft versions as a latest version: if the latest version is a draft, it will be shown, even if there are older non-draft versions.</li>   </ul>   As long as no version filters are used, each listed <em>webscript version</em> contains representations of the latest draft (`entities[]._links.draft`)  or latest published (`entities[]._links.published`) version (if existing and different).   Use the query parameter `showRelated` to include only a link (default `showRelated=link`) or a full representation (`showRelated=embed`).  ### List Latest Webscript Versions (with filter) When any of the _version filter_ query parameters are used, the response contains the _latest_ version per named <em>webscript</em> that satisfy the filters, but **without links**.  ### List All Webscript Versions When using `latest=false` (default when using the `namedVersion` filter), the listing contains _all_  <em>webscripts</em> versions that satisfy the query, possibly multiple versions per named <em>webscripts</em>. No HAL links are provided.  #### Filter on _status_ By default <em>webscript versions</em> with status  `undeployed` are **excluded** in all cases. Use the _version filter_ `status` to include/exclude a status from the results. By example,  > `?status=any&includeDeprecated=true&includeDraft=true&latest=false`  will list _ALL_ versions known to the function registry.  #### Version filter parameters The following query parameters are _version filters_ for the <em>webscript</em> listing: > `version`, `status`, `runtimeVersion`, `createdBy`, `createdBefore`, `createdAfter`, `updatedBy`, `updatedBefore`, `updatedAfter`, `nameVersion`, `deprecated`, `draft`
         :param query: URL Query parameters.
@@ -1902,15 +1866,14 @@
         :type query['latest']: bool
         :param query['showRelated'] (dict) <br> query.show_related (Query) : Sets the representation of related function versions (like the _latest_ draft and/or published) in the response. - `embed`: as full summary representation (in `_embedded`). - `link`: as HAL link in (in `_links`). - `none`: omitted.
         :type query['showRelated']: ShowRelatedType
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1921,22 +1884,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(ListQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": LatestWebscriptsResponseV2 if not select_path else Model,
@@ -1968,15 +1935,14 @@
         ],
         *,
         json: FunctionMeta | None = None,
         query: PatchMetadataQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetWebscriptResponseV2: ...
 
     @overload
     async def patch_metadata(
         self,
@@ -1986,15 +1952,14 @@
         ],
         *,
         json: FunctionMeta | None = None,
         query: PatchMetadataQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def patch_metadata(
         self,
@@ -2004,15 +1969,14 @@
         ],
         *,
         json: FunctionMeta | None = None,
         query: PatchMetadataQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def patch_metadata(
         self,
@@ -2022,15 +1986,14 @@
         ],
         *,
         json: FunctionMeta | None = None,
         query: PatchMetadataQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def patch_metadata(
         self,
@@ -2040,15 +2003,14 @@
         ],
         *,
         json: FunctionMeta | None = None,
         query: PatchMetadataQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def patch_metadata(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -2057,15 +2019,14 @@
         ],
         *,
         json: FunctionMeta | None = None,
         query: PatchMetadataQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetWebscriptResponseV2 | T | Response | Model:
         """Patch Webscript Metadata.
 
         Patch the metadata of a webscript version.
         :param name: The name of the function. (required)
@@ -2078,15 +2039,14 @@
         :type query: PatchMetadataQuery | QueryParamTypes, optional
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -2097,29 +2057,33 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
+        if json is not None and should_validate:
             body_adapter = TypeAdapter(Optional[FunctionMeta])
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(PatchMetadataQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": GetWebscriptResponseV2 if not select_path else Model,
@@ -2150,15 +2114,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: PublishQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostWebscriptJobSyncResponseV2 | PostWebscriptJobAsyncResponseV2: ...
 
     @overload
     async def publish(
         self,
@@ -2167,15 +2130,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: PublishQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def publish(
         self,
@@ -2184,15 +2146,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: PublishQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def publish(
         self,
@@ -2201,15 +2162,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: PublishQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def publish(
         self,
@@ -2218,15 +2178,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: PublishQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def publish(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -2234,15 +2193,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: PublishQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> (
         PostWebscriptJobSyncResponseV2
         | PostWebscriptJobAsyncResponseV2
         | T
         | Response
@@ -2267,15 +2225,14 @@
         :type query['deprecatePrevious']: DeprecatePreviousPolicy
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -2286,25 +2243,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(PublishQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": PostWebscriptJobSyncResponseV2 if not select_path else Model,
@@ -2336,15 +2297,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RebuildQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> RebuildWebscriptSyncResponseV2 | RebuildWebscriptAsyncResponseV2: ...
 
     @overload
     async def rebuild(
         self,
@@ -2353,15 +2313,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RebuildQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def rebuild(
         self,
@@ -2370,15 +2329,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RebuildQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def rebuild(
         self,
@@ -2387,15 +2345,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RebuildQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def rebuild(
         self,
@@ -2404,15 +2361,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RebuildQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def rebuild(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -2420,15 +2376,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RebuildQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> (
         RebuildWebscriptSyncResponseV2
         | RebuildWebscriptAsyncResponseV2
         | T
         | Response
@@ -2439,35 +2394,34 @@
         Rebuild and deploy a webscript with the original or updated base image.
         :param name: The name of the function. (required)
         :type name: str
         :param version: The version of the function. (required)
         :type version: str
         :param query: URL Query parameters.
         :type query: RebuildQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.
-        :type query['scaleToZero']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['dryRun'] (dict) <br> query.dry_run (Query) : If set to <code>true</code>, checks whether rebuild jobs are needed, but do not start any jobs.
         :type query['dryRun']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param query['upgrade'] (dict) <br> query.upgrade (Query) : If set, force a rebuild with the given <em>runtime</em> version selection policy. <ul>  <li><code>same</code> <b>patch</b> version.   This should only include backward compatible upgrades.  </li>  <li><code>minor</code> <b>major</b> version.   This might include an upgrade of e.g. the language runtime and/or provided   dependencies that could break compatiblity with the function. .</li> </ul>
         :type query['upgrade']: RebuildPolicy
         :param query['forceVersion'] (dict) <br> query.force_version (Query) : If set, force a rebuild with the given runtime version (including downgrades). This parameter is mutually exclusive to the `upgrade` parameter.
         :type query['forceVersion']: str
         :param query['ignoreChecks'] (dict) <br> query.ignore_checks (Query) : If set to true, checks that normally prevent a rebuild are overriden. These checks include: * function state in `pending`, `running`, `failed` or `undeployed` * backoff period due to recent failures * usage of deprecated dependencies * running jobs on entity * the `dryRun` option
         :type query['ignoreChecks']: bool
+        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful (re-)deployment. If not set, the function is scaled to zero only if it was not active before this command.
+        :type query['scaleToZero']: bool
         :param query['skipRebuild'] (dict) <br> query.skip_rebuild (Query) : If set, the function will not be rebuild. Always uses the current runtime version when re-deploying/re-verifying the function.
         :type query['skipRebuild']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -2478,25 +2432,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(RebuildQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": RebuildWebscriptSyncResponseV2 if not select_path else Model,
@@ -2528,15 +2486,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RemoveVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> UndeployedResponseV2 | UndeploySubmittedResponseV2: ...
 
     @overload
     async def remove_version(
         self,
@@ -2545,15 +2502,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RemoveVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def remove_version(
         self,
@@ -2562,15 +2518,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RemoveVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def remove_version(
         self,
@@ -2579,15 +2534,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RemoveVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def remove_version(
         self,
@@ -2596,15 +2550,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RemoveVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def remove_version(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -2612,15 +2565,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: RemoveVersionQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> UndeployedResponseV2 | UndeploySubmittedResponseV2 | T | Response | Model:
         """Remove Webscript Version.
 
         Deprecate, undeploy and/or remove a <em>webscript</em> version.    By default, a `DELETE`    * _deprecates_ the webscript version(s): they are no longer included in listings by default.   * _undeploys_ the webscript version(s) with delay: the function can no longer be invoked, the small delay allows     other services to discover the removal.   * _removes_ the version(s) from the plug registry.    Use `?force=true` to immediately _undeploy_ and _remove_ without delay.    Use `?undeploy=true` to undeploy, but keep the webscript version registered in a `undeployed` state.   An `undeployed` version can later be restored by a _rebuild_ action.
         :param name: The name of the function. (required)
@@ -2637,15 +2589,14 @@
         :type query['force']: bool
         :param query['undeploy'] (dict) <br> query.undeploy (Query) : If `true`, the `DELETE` operation * undeploys the (openfaas) function: it becomes no longer available for invocation. * does NOT remove the function from registry: it stays in an `undeployed` status.  All assets and definitions are retained, so the version can be restored later with a  _rebuild_ action.  If `false`, the `DELETE` operation * _only_ marks the plug function as _deprecated_, the function remains active but is removed from the default listings.   This also applies to _draft_ versions.  This parameter is incompatible with `force=true`.  If not set the default behaviour applies: * _draft_ versions are _undeployed_ and _removed_ from registry. * non-_draft_ versions are marked _deprecated_ only.
         :type query['undeploy']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -2656,25 +2607,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(RemoveVersionQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": UndeployedResponseV2 if not select_path else Model,
@@ -2703,84 +2658,78 @@
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: RemoveVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> UndeployedResponseV2 | UndeploySubmittedResponseV2: ...
 
     @overload
     async def remove_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: RemoveVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def remove_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: RemoveVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def remove_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: RemoveVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def remove_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: RemoveVersionsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def remove_versions(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
         *,
         query: RemoveVersionsQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> UndeployedResponseV2 | UndeploySubmittedResponseV2 | T | Response | Model:
         """Remove Webscript.
 
         Deprecate, undeploy and/or remove all versions of this named <em>webscript</em>.    By default, a `DELETE`    * _deprecates_ the webscript version(s): they are no longer included in listings by default.   * _undeploys_ the webscript version(s) with delay: the function can no longer be invoked, the small delay allows     other services to discover the removal.   * _removes_ the version(s) from the plug registry.    Use `?force=true` to immediately _undeploy_ and _remove_ without delay.    Use `?undeploy=true` to undeploy, but keep the webscript version registered in a `undeployed` state.   An `undeployed` version can later be restored by a _rebuild_ action.
         :param name: The name of the function. (required)
@@ -2795,15 +2744,14 @@
         :type query['force']: bool
         :param query['undeploy'] (dict) <br> query.undeploy (Query) : If `true`, the `DELETE` operation * undeploys the (openfaas) function: it becomes no longer available for invocation. * does NOT remove the function from registry: it stays in an `undeployed` status.  All assets and definitions are retained, so the version can be restored later with a  _rebuild_ action.  If `false`, the `DELETE` operation * _only_ marks the plug function as _deprecated_, the function remains active but is removed from the default listings.   This also applies to _draft_ versions.  This parameter is incompatible with `force=true`.  If not set the default behaviour applies: * _draft_ versions are _undeployed_ and _removed_ from registry. * non-_draft_ versions are marked _deprecated_ only.
         :type query['undeploy']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -2814,24 +2762,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(RemoveVersionsQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": UndeployedResponseV2 if not select_path else Model,
@@ -2872,15 +2824,14 @@
         content: Annotated[
             RequestContent | None, Field(description="A single asset file.")
         ] = None,
         query: UpdateAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostWebscriptJobSyncResponseV2 | PostWebscriptJobAsyncResponseV2: ...
 
     @overload
     async def update_asset(
         self,
@@ -2898,15 +2849,14 @@
         content: Annotated[
             RequestContent | None, Field(description="A single asset file.")
         ] = None,
         query: UpdateAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def update_asset(
         self,
@@ -2924,15 +2874,14 @@
         content: Annotated[
             RequestContent | None, Field(description="A single asset file.")
         ] = None,
         query: UpdateAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def update_asset(
         self,
@@ -2950,15 +2899,14 @@
         content: Annotated[
             RequestContent | None, Field(description="A single asset file.")
         ] = None,
         query: UpdateAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def update_asset(
         self,
@@ -2976,15 +2924,14 @@
         content: Annotated[
             RequestContent | None, Field(description="A single asset file.")
         ] = None,
         query: UpdateAssetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def update_asset(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -3001,15 +2948,14 @@
         content: Annotated[
             RequestContent | None, Field(description="A single asset file.")
         ] = None,
         query: UpdateAssetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> (
         PostWebscriptJobSyncResponseV2
         | PostWebscriptJobAsyncResponseV2
         | T
         | Response
@@ -3024,31 +2970,26 @@
         :type version: str
         :param wildcard: Full path or path prefix of the asset within the archive (required)
         :type wildcard: str
         :param content: A single asset file.
         :type content: ContentRequest, optional
         :param query: URL Query parameters.
         :type query: UpdateAssetQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['chown'] (dict) <br> query.chown (Query) : If set, ownership of the draft function is transferred to the current user.
         :type query['chown']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -3059,27 +3000,31 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
             "wildcard": str(wildcard),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
         body_args["content"] = content
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(UpdateAssetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": PostWebscriptJobSyncResponseV2 if not select_path else Model,
@@ -3122,15 +3067,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: UpdateAssetsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> PostWebscriptJobSyncResponseV2 | PostWebscriptJobAsyncResponseV2: ...
 
     @overload
     async def update_assets(
         self,
@@ -3148,15 +3092,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: UpdateAssetsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def update_assets(
         self,
@@ -3174,15 +3117,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: UpdateAssetsQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def update_assets(
         self,
@@ -3200,15 +3142,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: UpdateAssetsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def update_assets(
         self,
@@ -3226,15 +3167,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: UpdateAssetsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def update_assets(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -3251,15 +3191,14 @@
         files: Annotated[
             RequestFiles | None, Field(description="Multipart file upload")
         ] = None,
         query: UpdateAssetsQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> (
         PostWebscriptJobSyncResponseV2
         | PostWebscriptJobAsyncResponseV2
         | T
         | Response
@@ -3274,31 +3213,26 @@
         :type version: str
         :param content: The assets for a <em>webscript</em> function can be provided as either   <ul>     <li>a single <em>tar</em> archive (optionally compressed), with one of the content types      <code>application/octet-stream</code>, <code>application/tar</code>, <code>application/tar+gzip</code>, <code>application/x-gzip</code>, <code>application/x-tar</code>, <code>application/gzip</code></li>     <li>separate files in a <code>multipart/form-data</code> request</li>   </ul>    The provided assets will be added to the <em>webscript</em> function's collection of existing assets,   replacing any existing assets with the same name.    Please note that it is not allowed to update the webscript.json</code> json file with a changed value for any of the    <code>name</code>, <code>version</code> and/or <code>runtime</code> attributes.    For each <em>runtime</em> other files are supported.
         :type content: ContentRequest, optional
         :param files: The files of a `content-type: multipart/form-data` request.
         :type files: FilesRequest, optional
         :param query: URL Query parameters.
         :type query: UpdateAssetsQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['chown'] (dict) <br> query.chown (Query) : If set, ownership of the draft function is transferred to the current user.
         :type query['chown']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -3309,27 +3243,31 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
         body_args["content"] = content
         body_args["files"] = files
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(UpdateAssetsQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": PostWebscriptJobSyncResponseV2 if not select_path else Model,
@@ -3363,15 +3301,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: VerifyQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> VerifyWebscriptSyncResponseV2 | PostWebscriptJobAsyncResponseV2: ...
 
     @overload
     async def verify(
         self,
@@ -3380,15 +3317,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: VerifyQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def verify(
         self,
@@ -3397,15 +3333,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: VerifyQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def verify(
         self,
@@ -3414,15 +3349,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: VerifyQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def verify(
         self,
@@ -3431,15 +3365,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: VerifyQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def verify(
         self,
         name: Annotated[StrictStr, Field(description="The name of the function.")],
@@ -3447,15 +3380,14 @@
             str, Field(strict=True, description="The version of the function.")
         ],
         *,
         query: VerifyQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> (
         VerifyWebscriptSyncResponseV2
         | PostWebscriptJobAsyncResponseV2
         | T
         | Response
@@ -3466,23 +3398,22 @@
         Verify health of webscript deployed on openfaas.
         :param name: The name of the function. (required)
         :type name: str
         :param version: The version of the function. (required)
         :type version: str
         :param query: URL Query parameters.
         :type query: VerifyQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.
-        :type query['scaleToZero']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
+        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.
+        :type query['scaleToZero']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -3493,25 +3424,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
             "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(VerifyQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": VerifyWebscriptSyncResponseV2 if not select_path else Model,
```

### Comparing `waylay_sdk_registry-2.13.0b20240423/src/waylay/services/registry/service/service.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/service/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """Registry Service."""
 
 from waylay.sdk import ApiClient, WaylayService
 
-from ..api.about_api import AboutApi
+from ..api.default_api import DefaultApi
 from ..api.jobs_api import JobsApi
 from ..api.models_api import ModelsApi
 from ..api.plugs_api import PlugsApi
 from ..api.runtimes_api import RuntimesApi
 from ..api.schemas_api import SchemasApi
 from ..api.webscripts_api import WebscriptsApi
 
 
 class RegistryService(WaylayService):
     """Registry Service Class."""
 
     name = "registry"
     title = "Registry Service"
 
-    about: AboutApi
     jobs: JobsApi
     models: ModelsApi
     plugs: PlugsApi
     runtimes: RuntimesApi
     schemas: SchemasApi
     webscripts: WebscriptsApi
+    default: DefaultApi
 
     def __init__(self, api_client: ApiClient):
         """Create the registry service."""
 
         super().__init__(api_client)
-        self.about = AboutApi(api_client)
         self.jobs = JobsApi(api_client)
         self.models = ModelsApi(api_client)
         self.plugs = PlugsApi(api_client)
         self.runtimes = RuntimesApi(api_client)
         self.schemas = SchemasApi(api_client)
         self.webscripts = WebscriptsApi(api_client)
+        self.default = DefaultApi(api_client)
```

### Comparing `waylay_sdk_registry-2.13.0b20240423/src/waylay_sdk_registry.egg-info/PKG-INFO` & `waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-registry
-Version: 2.13.0b20240423
+Version: 2.13.0rc0
 Summary: Waylay Function Registry
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,22 +13,21 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-registry-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/registry.html
 Keywords: Waylay Function Registry
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.1
+Requires-Dist: waylay-sdk~=0.0.4rc5
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -46,52 +45,57 @@
 Provides-Extra: types
 Requires-Dist: waylay-sdk-registry-types; extra == "types"
 
 # Waylay Registry Service
 V2 API to build and deploy Waylay functions (plugs, webscripts, BYOML models).
 
 This Python package is automatically generated based on the 
-Waylay Registry OpenAPI specification (API version: 2.13.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/registry.html).
+Waylay Registry OpenAPI specification (API version: 2.13.0-beta.0)
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Registry api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Registry api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-registry-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-registry is included in:
-- ```pip install waylay-sdk-core[registry]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[registry]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-registry and waylay-sdk-registry-types are included in:
-- ```pip install waylay-sdk-core[registry,registry-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[registry,registry-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-registry-types` is installed
-from waylay.services.registry.models.root_page_response import RootPageResponse
+from registry.models.function_type import FunctionType
+from registry.models.job_state_result import JobStateResult
+from registry.models.job_type_schema import JobTypeSchema
+from registry.models.jobs_response import JobsResponse
 try:
-    # Get Service Status
-    # calls `GET /registry/v2/`
-    api_response = await waylay_client.registry.about.get(
+    # List Jobs
+    # calls `GET /registry/v2/jobs/`
+    api_response = await waylay_client.registry.jobs.list(
+        # query parameters:
+        query = {
+        },
     )
-    print("The response of registry.about.get:\n")
+    print("The response of registry.jobs.list:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling registry.about.get: %s\n" % e)
+    print("Exception when calling registry.jobs.list: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_registry-2.13.0b20240423/src/waylay_sdk_registry.egg-info/SOURCES.txt` & `waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENSE.txt
 README.md
 pyproject.toml
 src/waylay/services/registry/api/__init__.py
-src/waylay/services/registry/api/about_api.py
+src/waylay/services/registry/api/default_api.py
 src/waylay/services/registry/api/jobs_api.py
 src/waylay/services/registry/api/models_api.py
 src/waylay/services/registry/api/plugs_api.py
 src/waylay/services/registry/api/py.typed
 src/waylay/services/registry/api/runtimes_api.py
 src/waylay/services/registry/api/schemas_api.py
 src/waylay/services/registry/api/webscripts_api.py
```

