# Comparing `tmp/edgegap_service-1.2.0.tar.gz` & `tmp/edgegap_service-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_service-1.2.0.tar", max compression
+gzip compressed data, was "edgegap_service-1.5.0.tar", max compression
```

## Comparing `edgegap_service-1.2.0.tar` & `edgegap_service-1.5.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     1993 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/LICENSE
--rw-r--r--   0        0        0     2188 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/README.md
--rw-r--r--   0        0        0       17 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/BUILD
--rw-r--r--   0        0        0      165 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/__init__.py
--rw-r--r--   0        0        0     2657 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/_configuration.py
--rw-r--r--   0        0        0      735 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/_documentation.py
--rw-r--r--   0        0        0      717 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/_environment.py
--rw-r--r--   0        0        0     2213 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/_logging.py
--rw-r--r--   0        0        0     2890 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/_scheduling.py
--rw-r--r--   0        0        0     7661 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/_service.py
--rw-r--r--   0        0        0      739 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/_templating.py
--rw-r--r--   0        0        0       17 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/BUILD
--rw-r--r--   0        0        0      102 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/__init__.py
--rw-r--r--   0        0        0     1453 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/_health.py
--rw-r--r--   0        0        0      394 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/_model.py
--rw-r--r--   0        0        0       17 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/checks/BUILD
--rw-r--r--   0        0        0      235 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/checks/__init__.py
--rw-r--r--   0        0        0      594 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/checks/_consul.py
--rw-r--r--   0        0        0      740 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/checks/_database.py
--rw-r--r--   0        0        0      590 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/checks/_interface.py
--rw-r--r--   0        0        0      329 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/checks/_model.py
--rw-r--r--   0        0        0     1880 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/static/html/index.html
--rw-r--r--   0        0        0     4286 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/static/images/favicon.ico
--rw-r--r--   0        0        0      972 2024-05-01 17:52:38.063483 edgegap_service-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 edgegap_service-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2188 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/README.md
+-rw-r--r--   0        0        0       17 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/BUILD
+-rw-r--r--   0        0        0      225 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/__init__.py
+-rw-r--r--   0        0        0     2656 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/_configuration.py
+-rw-r--r--   0        0        0      735 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/_documentation.py
+-rw-r--r--   0        0        0      717 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/_environment.py
+-rw-r--r--   0        0        0     2890 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/_scheduling.py
+-rw-r--r--   0        0        0     7661 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/_service.py
+-rw-r--r--   0        0        0      739 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/_templating.py
+-rw-r--r--   0        0        0       17 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/BUILD
+-rw-r--r--   0        0        0      102 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/__init__.py
+-rw-r--r--   0        0        0     1453 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/_health.py
+-rw-r--r--   0        0        0      394 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/_model.py
+-rw-r--r--   0        0        0       17 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/checks/BUILD
+-rw-r--r--   0        0        0      235 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/checks/__init__.py
+-rw-r--r--   0        0        0      594 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/checks/_consul.py
+-rw-r--r--   0        0        0      740 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/checks/_database.py
+-rw-r--r--   0        0        0      590 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/checks/_interface.py
+-rw-r--r--   0        0        0      329 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/checks/_model.py
+-rw-r--r--   0        0        0      152 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/logging/__init__.py
+-rw-r--r--   0        0        0     2135 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/logging/_configuration.py
+-rw-r--r--   0        0        0     1656 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/logging/_logger.py
+-rw-r--r--   0        0        0     1880 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/static/html/index.html
+-rw-r--r--   0        0        0     4286 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/static/images/favicon.ico
+-rw-r--r--   0        0        0      972 2024-05-02 18:20:24.167778 edgegap_service-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 edgegap_service-1.5.0/PKG-INFO
```

### Comparing `edgegap_service-1.2.0/LICENSE` & `edgegap_service-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.2.0/README.md` & `edgegap_service-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.2.0/edgegap_service/_configuration.py` & `edgegap_service-1.5.0/edgegap_service/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from edgegap_scheduling import Scheduler
 from edgegap_settings import ProjectBaseSettings, SettingsFactory
 from fastapi import APIRouter
 from pydantic import BaseModel, ConfigDict, Field
 
 from ._environment import EnvironmentConfiguration
-from ._logging import LoggingConfiguration
 from .health.checks import CheckInterface
+from .logging import LoggingConfiguration
 
 
 class ServiceConfiguration(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
     name: str = Field(..., description='The name of the Service')
     version: str = Field(..., description='The version of the Service')
     description: str = Field(..., description='The description of the Service')
```

### Comparing `edgegap_service-1.2.0/edgegap_service/_documentation.py` & `edgegap_service-1.5.0/edgegap_service/_documentation.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.2.0/edgegap_service/_environment.py` & `edgegap_service-1.5.0/edgegap_service/_environment.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.2.0/edgegap_service/_logging.py` & `edgegap_service-1.5.0/edgegap_service/logging/_configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 from edgegap_settings import SettingsFactory
 from pydantic import BaseModel
 
-from ._environment import EnvironmentConfiguration
+from .._environment import EnvironmentConfiguration
 
 env_config: EnvironmentConfiguration = SettingsFactory.from_settings(EnvironmentConfiguration)
 
 
 class LoggingConfiguration(BaseModel):
-    """Logging configuration to be set for the server"""
-
-    # Logging config
     version: int = 1
     disable_existing_loggers: bool = False
     formatters: dict = {
         'default': {
             '()': 'edgegap_logging.DefaultFormatter',
             'fmt': env_config.log_format,
         },
         'access': {
-            '()': 'edgegap_logging.AccessFormatter',
+            '()': 'edgegap_service.AccessFormatter',
             'fmt': env_config.log_access_format,
         },
     }
     handlers: dict = {
         'default': {
             'formatter': 'default',
             'class': 'logging.StreamHandler',
```

### Comparing `edgegap_service-1.2.0/edgegap_service/_scheduling.py` & `edgegap_service-1.5.0/edgegap_service/_scheduling.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.2.0/edgegap_service/_service.py` & `edgegap_service-1.5.0/edgegap_service/_service.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.2.0/edgegap_service/_templating.py` & `edgegap_service-1.5.0/edgegap_service/_templating.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.2.0/edgegap_service/health/_health.py` & `edgegap_service-1.5.0/edgegap_service/health/_health.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.2.0/edgegap_service/health/checks/_consul.py` & `edgegap_service-1.5.0/edgegap_service/health/checks/_consul.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.2.0/edgegap_service/health/checks/_database.py` & `edgegap_service-1.5.0/edgegap_service/health/checks/_database.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.2.0/edgegap_service/health/checks/_interface.py` & `edgegap_service-1.5.0/edgegap_service/health/checks/_interface.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.2.0/edgegap_service/static/html/index.html` & `edgegap_service-1.5.0/edgegap_service/static/html/index.html`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.2.0/edgegap_service/static/images/favicon.ico` & `edgegap_service-1.5.0/edgegap_service/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.2.0/pyproject.toml` & `edgegap_service-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-service"
-version = "1.2.0"
+version = "1.5.0"
 description = "The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 include = ["static/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `edgegap_service-1.2.0/PKG-INFO` & `edgegap_service-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-service
-Version: 1.2.0
+Version: 1.5.0
 Summary: The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

