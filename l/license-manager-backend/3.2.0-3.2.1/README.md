# Comparing `tmp/license_manager_backend-3.2.0.tar.gz` & `tmp/license_manager_backend-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_manager_backend-3.2.0.tar", max compression
+gzip compressed data, was "license_manager_backend-3.2.1.tar", max compression
```

## Comparing `license_manager_backend-3.2.0.tar` & `license_manager_backend-3.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1829 2024-04-29 19:53:20.531443 license_manager_backend-3.2.0/README.md
--rw-r--r--   0        0        0       60 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/__init__.py
--rw-r--r--   0        0        0      929 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/cruds/__init__.py
--rw-r--r--   0        0        0     3078 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/cruds/booking.py
--rw-r--r--   0        0        0     2157 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/cruds/configuration.py
--rw-r--r--   0        0        0     6451 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/cruds/feature.py
--rw-r--r--   0        0        0     6101 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/cruds/generic.py
--rw-r--r--   0        0        0        0 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/models/__init__.py
--rw-r--r--   0        0        0     1362 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/models/booking.py
--rw-r--r--   0        0        0     1703 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/models/configuration.py
--rw-r--r--   0        0        0      575 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/models/crud_base.py
--rw-r--r--   0        0        0     1992 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/models/feature.py
--rw-r--r--   0        0        0     1216 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/models/job.py
--rw-r--r--   0        0        0     1080 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/models/license_server.py
--rw-r--r--   0        0        0      777 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/models/product.py
--rw-r--r--   0        0        0        0 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/routes/__init__.py
--rw-r--r--   0        0        0     2220 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/routes/bookings.py
--rw-r--r--   0        0        0     9532 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/routes/configurations.py
--rw-r--r--   0        0        0     3811 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/routes/features.py
--rw-r--r--   0        0        0     7185 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/routes/jobs.py
--rw-r--r--   0        0        0     3565 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/routes/license_servers.py
--rw-r--r--   0        0        0     2818 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/routes/products.py
--rw-r--r--   0        0        0        0 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/schemas/__init__.py
--rw-r--r--   0        0        0      313 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/schemas/base.py
--rw-r--r--   0        0        0     1797 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/schemas/booking.py
--rw-r--r--   0        0        0     6361 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/schemas/configuration.py
--rw-r--r--   0        0        0     5736 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/schemas/feature.py
--rw-r--r--   0        0        0     3600 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/schemas/job.py
--rw-r--r--   0        0        0     4420 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/schemas/license_server.py
--rw-r--r--   0        0        0      984 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/schemas/product.py
--rw-r--r--   0        0        0     1821 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/config.py
--rw-r--r--   0        0        0      489 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/constants.py
--rw-r--r--   0        0        0     7203 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/database.py
--rw-r--r--   0        0        0     2850 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/main.py
--rw-r--r--   0        0        0     1481 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/permissions.py
--rw-r--r--   0        0        0     3349 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/security.py
--rw-r--r--   0        0        0     1099 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/version.py
--rw-r--r--   0        0        0     2021 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     3140 1970-01-01 00:00:00.000000 license_manager_backend-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1829 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/README.md
+-rw-r--r--   0        0        0       60 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/__init__.py
+-rw-r--r--   0        0        0      929 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/cruds/__init__.py
+-rw-r--r--   0        0        0     3078 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/cruds/booking.py
+-rw-r--r--   0        0        0     2157 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/cruds/configuration.py
+-rw-r--r--   0        0        0     6451 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/cruds/feature.py
+-rw-r--r--   0        0        0     6101 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/cruds/generic.py
+-rw-r--r--   0        0        0        0 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/models/__init__.py
+-rw-r--r--   0        0        0     1362 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/models/booking.py
+-rw-r--r--   0        0        0     1703 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/models/configuration.py
+-rw-r--r--   0        0        0      575 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/models/crud_base.py
+-rw-r--r--   0        0        0     1992 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/models/feature.py
+-rw-r--r--   0        0        0     1216 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/models/job.py
+-rw-r--r--   0        0        0     1080 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/models/license_server.py
+-rw-r--r--   0        0        0      777 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/models/product.py
+-rw-r--r--   0        0        0        0 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/routes/__init__.py
+-rw-r--r--   0        0        0     2220 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/routes/bookings.py
+-rw-r--r--   0        0        0     9532 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/routes/configurations.py
+-rw-r--r--   0        0        0     3811 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/routes/features.py
+-rw-r--r--   0        0        0     7185 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/routes/jobs.py
+-rw-r--r--   0        0        0     3565 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/routes/license_servers.py
+-rw-r--r--   0        0        0     2818 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/routes/products.py
+-rw-r--r--   0        0        0        0 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/schemas/__init__.py
+-rw-r--r--   0        0        0      313 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/schemas/base.py
+-rw-r--r--   0        0        0     1797 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/schemas/booking.py
+-rw-r--r--   0        0        0     6361 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/schemas/configuration.py
+-rw-r--r--   0        0        0     5736 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/schemas/feature.py
+-rw-r--r--   0        0        0     3600 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/schemas/job.py
+-rw-r--r--   0        0        0     4420 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/schemas/license_server.py
+-rw-r--r--   0        0        0      984 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/api/schemas/product.py
+-rw-r--r--   0        0        0     1821 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/config.py
+-rw-r--r--   0        0        0      489 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/constants.py
+-rw-r--r--   0        0        0     7203 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/database.py
+-rw-r--r--   0        0        0     2850 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/main.py
+-rw-r--r--   0        0        0     1481 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/permissions.py
+-rw-r--r--   0        0        0     3349 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/security.py
+-rw-r--r--   0        0        0     1099 2024-05-02 17:08:19.669423 license_manager_backend-3.2.1/lm_api/version.py
+-rw-r--r--   0        0        0     2021 2024-05-02 17:08:19.673423 license_manager_backend-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3140 1970-01-01 00:00:00.000000 license_manager_backend-3.2.1/PKG-INFO
```

### Comparing `license_manager_backend-3.2.0/README.md` & `license_manager_backend-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/__init__.py` & `license_manager_backend-3.2.1/lm_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/cruds/booking.py` & `license_manager_backend-3.2.1/lm_api/api/cruds/booking.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/cruds/configuration.py` & `license_manager_backend-3.2.1/lm_api/api/cruds/configuration.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/cruds/feature.py` & `license_manager_backend-3.2.1/lm_api/api/cruds/feature.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/cruds/generic.py` & `license_manager_backend-3.2.1/lm_api/api/cruds/generic.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/models/booking.py` & `license_manager_backend-3.2.1/lm_api/api/models/booking.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/models/configuration.py` & `license_manager_backend-3.2.1/lm_api/api/models/configuration.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/models/crud_base.py` & `license_manager_backend-3.2.1/lm_api/api/models/crud_base.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/models/feature.py` & `license_manager_backend-3.2.1/lm_api/api/models/feature.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/models/job.py` & `license_manager_backend-3.2.1/lm_api/api/models/job.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/models/license_server.py` & `license_manager_backend-3.2.1/lm_api/api/models/license_server.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/models/product.py` & `license_manager_backend-3.2.1/lm_api/api/models/product.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/routes/bookings.py` & `license_manager_backend-3.2.1/lm_api/api/routes/bookings.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/routes/configurations.py` & `license_manager_backend-3.2.1/lm_api/api/routes/configurations.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/routes/features.py` & `license_manager_backend-3.2.1/lm_api/api/routes/features.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/routes/jobs.py` & `license_manager_backend-3.2.1/lm_api/api/routes/jobs.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/routes/license_servers.py` & `license_manager_backend-3.2.1/lm_api/api/routes/license_servers.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/routes/products.py` & `license_manager_backend-3.2.1/lm_api/api/routes/products.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/schemas/booking.py` & `license_manager_backend-3.2.1/lm_api/api/schemas/booking.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/schemas/configuration.py` & `license_manager_backend-3.2.1/lm_api/api/schemas/configuration.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/schemas/feature.py` & `license_manager_backend-3.2.1/lm_api/api/schemas/feature.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/schemas/job.py` & `license_manager_backend-3.2.1/lm_api/api/schemas/job.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/schemas/license_server.py` & `license_manager_backend-3.2.1/lm_api/api/schemas/license_server.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/api/schemas/product.py` & `license_manager_backend-3.2.1/lm_api/api/schemas/product.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/config.py` & `license_manager_backend-3.2.1/lm_api/config.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/database.py` & `license_manager_backend-3.2.1/lm_api/database.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/main.py` & `license_manager_backend-3.2.1/lm_api/main.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/permissions.py` & `license_manager_backend-3.2.1/lm_api/permissions.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/security.py` & `license_manager_backend-3.2.1/lm_api/security.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/lm_api/version.py` & `license_manager_backend-3.2.1/lm_api/version.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.2.0/pyproject.toml` & `license_manager_backend-3.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "license-manager-backend"
-version = "3.2.0"
+version = "3.2.1"
 description = "Provides an API for managing license data"
 authors = ["OmniVector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/license-manager"
 documentation = "https://omnivector-solutions.github.io/license-manager/"
 packages = [{ include = "lm_api" }]
```

### Comparing `license_manager_backend-3.2.0/PKG-INFO` & `license_manager_backend-3.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license-manager-backend
-Version: 3.2.0
+Version: 3.2.1
 Summary: Provides an API for managing license data
 Home-page: https://github.com/omnivector-solutions/license-manager
 License: MIT
 Author: OmniVector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

