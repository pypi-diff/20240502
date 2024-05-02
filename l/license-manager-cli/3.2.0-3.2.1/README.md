# Comparing `tmp/license_manager_cli-3.2.0.tar.gz` & `tmp/license_manager_cli-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_manager_cli-3.2.0.tar", max compression
+gzip compressed data, was "license_manager_cli-3.2.1.tar", max compression
```

## Comparing `license_manager_cli-3.2.0.tar` & `license_manager_cli-3.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1082 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/LICENSE
--rw-r--r--   0        0        0     1719 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/README.md
--rw-r--r--   0        0        0        0 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/__init__.py
--rw-r--r--   0        0        0    10455 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/auth.py
--rw-r--r--   0        0        0     2897 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/config.py
--rw-r--r--   0        0        0      565 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/constants.py
--rw-r--r--   0        0        0     2569 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/exceptions.py
--rw-r--r--   0        0        0      675 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/logs.py
--rw-r--r--   0        0        0     5998 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/main.py
--rw-r--r--   0        0        0     4558 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/render.py
--rw-r--r--   0        0        0     7143 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/requests.py
--rw-r--r--   0        0        0     1760 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/schemas.py
--rw-r--r--   0        0        0        0 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/subapps/__init__.py
--rw-r--r--   0        0        0     1625 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/subapps/bookings.py
--rw-r--r--   0        0        0     5603 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/subapps/configurations.py
--rw-r--r--   0        0        0     5388 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/subapps/features.py
--rw-r--r--   0        0        0     2249 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/subapps/jobs.py
--rw-r--r--   0        0        0     4329 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/subapps/license_servers.py
--rw-r--r--   0        0        0     3907 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/subapps/products.py
--rw-r--r--   0        0        0     1147 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/text_tools.py
--rw-r--r--   0        0        0     3802 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/lm_cli/time_loop.py
--rw-r--r--   0        0        0     1597 2024-04-29 19:53:22.768100 license_manager_cli-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     2797 1970-01-01 00:00:00.000000 license_manager_cli-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/LICENSE
+-rw-r--r--   0        0        0     1719 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/__init__.py
+-rw-r--r--   0        0        0    10455 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/auth.py
+-rw-r--r--   0        0        0     2897 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/config.py
+-rw-r--r--   0        0        0      565 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/constants.py
+-rw-r--r--   0        0        0     2569 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/exceptions.py
+-rw-r--r--   0        0        0      675 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/logs.py
+-rw-r--r--   0        0        0     5998 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/main.py
+-rw-r--r--   0        0        0     4558 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/render.py
+-rw-r--r--   0        0        0     7143 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/requests.py
+-rw-r--r--   0        0        0     1760 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/schemas.py
+-rw-r--r--   0        0        0        0 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/subapps/__init__.py
+-rw-r--r--   0        0        0     1625 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/subapps/bookings.py
+-rw-r--r--   0        0        0     5603 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/subapps/configurations.py
+-rw-r--r--   0        0        0     5388 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/subapps/features.py
+-rw-r--r--   0        0        0     2249 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/subapps/jobs.py
+-rw-r--r--   0        0        0     4329 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/subapps/license_servers.py
+-rw-r--r--   0        0        0     3907 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/subapps/products.py
+-rw-r--r--   0        0        0     1147 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/text_tools.py
+-rw-r--r--   0        0        0     3802 2024-05-02 17:08:19.268052 license_manager_cli-3.2.1/lm_cli/time_loop.py
+-rw-r--r--   0        0        0     1597 2024-05-02 17:08:19.272052 license_manager_cli-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2797 1970-01-01 00:00:00.000000 license_manager_cli-3.2.1/PKG-INFO
```

### Comparing `license_manager_cli-3.2.0/LICENSE` & `license_manager_cli-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/README.md` & `license_manager_cli-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/lm_cli/auth.py` & `license_manager_cli-3.2.1/lm_cli/auth.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/lm_cli/config.py` & `license_manager_cli-3.2.1/lm_cli/config.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/lm_cli/constants.py` & `license_manager_cli-3.2.1/lm_cli/constants.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/lm_cli/exceptions.py` & `license_manager_cli-3.2.1/lm_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/lm_cli/logs.py` & `license_manager_cli-3.2.1/lm_cli/logs.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/lm_cli/main.py` & `license_manager_cli-3.2.1/lm_cli/main.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/lm_cli/render.py` & `license_manager_cli-3.2.1/lm_cli/render.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/lm_cli/requests.py` & `license_manager_cli-3.2.1/lm_cli/requests.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/lm_cli/schemas.py` & `license_manager_cli-3.2.1/lm_cli/schemas.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/lm_cli/subapps/bookings.py` & `license_manager_cli-3.2.1/lm_cli/subapps/bookings.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/lm_cli/subapps/configurations.py` & `license_manager_cli-3.2.1/lm_cli/subapps/configurations.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/lm_cli/subapps/features.py` & `license_manager_cli-3.2.1/lm_cli/subapps/features.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/lm_cli/subapps/jobs.py` & `license_manager_cli-3.2.1/lm_cli/subapps/jobs.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/lm_cli/subapps/license_servers.py` & `license_manager_cli-3.2.1/lm_cli/subapps/license_servers.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/lm_cli/subapps/products.py` & `license_manager_cli-3.2.1/lm_cli/subapps/products.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/lm_cli/text_tools.py` & `license_manager_cli-3.2.1/lm_cli/text_tools.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/lm_cli/time_loop.py` & `license_manager_cli-3.2.1/lm_cli/time_loop.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-3.2.0/pyproject.toml` & `license_manager_cli-3.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "license-manager-cli"
-version = "3.2.0"
+version = "3.2.1"
 description = "License Manager CLI Client"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/license-manager"
 documentation = "https://omnivector-solutions.github.io/license-manager/"
 packages = [ { include = "lm_cli" } ]
```

### Comparing `license_manager_cli-3.2.0/PKG-INFO` & `license_manager_cli-3.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license-manager-cli
-Version: 3.2.0
+Version: 3.2.1
 Summary: License Manager CLI Client
 Home-page: https://github.com/omnivector-solutions/license-manager
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

