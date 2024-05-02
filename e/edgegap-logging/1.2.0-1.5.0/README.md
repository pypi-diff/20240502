# Comparing `tmp/edgegap_logging-1.2.0.tar.gz` & `tmp/edgegap_logging-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_logging-1.2.0.tar", max compression
+gzip compressed data, was "edgegap_logging-1.5.0.tar", max compression
```

## Comparing `edgegap_logging-1.2.0.tar` & `edgegap_logging-1.5.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1993 2024-05-01 17:52:18.963014 edgegap_logging-1.2.0/LICENSE
--rw-r--r--   0        0        0     2216 2024-05-01 17:52:18.963014 edgegap_logging-1.2.0/README.md
--rw-r--r--   0        0        0       17 2024-05-01 17:52:18.963014 edgegap_logging-1.2.0/edgegap_logging/BUILD
--rw-r--r--   0        0        0      222 2024-05-01 17:52:18.963014 edgegap_logging-1.2.0/edgegap_logging/__init__.py
--rw-r--r--   0        0        0      417 2024-05-01 17:52:18.963014 edgegap_logging-1.2.0/edgegap_logging/_format.py
--rw-r--r--   0        0        0     4058 2024-05-01 17:52:18.963014 edgegap_logging-1.2.0/edgegap_logging/_logging.py
--rw-r--r--   0        0        0      644 2024-05-01 17:52:27.963235 edgegap_logging-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 edgegap_logging-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-02 18:20:19.991672 edgegap_logging-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2216 2024-05-02 18:20:19.991672 edgegap_logging-1.5.0/README.md
+-rw-r--r--   0        0        0       17 2024-05-02 18:20:19.991672 edgegap_logging-1.5.0/edgegap_logging/BUILD
+-rw-r--r--   0        0        0      217 2024-05-02 18:20:19.991672 edgegap_logging-1.5.0/edgegap_logging/__init__.py
+-rw-r--r--   0        0        0      847 2024-05-02 18:20:19.991672 edgegap_logging-1.5.0/edgegap_logging/_configuration.py
+-rw-r--r--   0        0        0      939 2024-05-02 18:20:19.991672 edgegap_logging-1.5.0/edgegap_logging/_format.py
+-rw-r--r--   0        0        0     1299 2024-05-02 18:20:19.991672 edgegap_logging-1.5.0/edgegap_logging/_logging.py
+-rw-r--r--   0        0        0      647 2024-05-02 18:20:48.628400 edgegap_logging-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 edgegap_logging-1.5.0/PKG-INFO
```

### Comparing `edgegap_logging-1.2.0/LICENSE` & `edgegap_logging-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.2.0/README.md` & `edgegap_logging-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.2.0/pyproject.toml` & `edgegap_logging-1.5.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "edgegap-logging"
-version = "1.2.0"
+version = "1.5.0"
 description = "The Edgegap Logging library includes various tools and helpers for interacting with Standard Logging Formatter and Colored Logs. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-click = "^8.1.7"
 colorama = "^0.4.6"
+pydantic = "^2.7.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 pytest-cov = "^5.0.0"
 ruff = "^0.4.2"
 
 [build-system]
```

### Comparing `edgegap_logging-1.2.0/PKG-INFO` & `edgegap_logging-1.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: edgegap-logging
-Version: 1.2.0
+Version: 1.5.0
 Summary: The Edgegap Logging library includes various tools and helpers for interacting with Standard Logging Formatter and Colored Logs. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Edgegap Logging Library
 
 This is the README for the Edgegap Logging Helper, which is part of the Edgegap suite of helpers.
 This library provides utilities for interacting with Standard Logging Formatter and Colored Logs.
```

