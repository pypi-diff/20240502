# Comparing `tmp/edgegap_settings-1.2.0.tar.gz` & `tmp/edgegap_settings-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_settings-1.2.0.tar", max compression
+gzip compressed data, was "edgegap_settings-1.5.0.tar", max compression
```

## Comparing `edgegap_settings-1.2.0.tar` & `edgegap_settings-1.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1993 2024-05-01 17:52:18.963014 edgegap_settings-1.2.0/LICENSE
--rw-r--r--   0        0        0     2182 2024-05-01 17:52:18.963014 edgegap_settings-1.2.0/README.md
--rw-r--r--   0        0        0       17 2024-05-01 17:52:18.963014 edgegap_settings-1.2.0/edgegap_settings/BUILD
--rw-r--r--   0        0        0      359 2024-05-01 17:52:18.963014 edgegap_settings-1.2.0/edgegap_settings/__init__.py
--rw-r--r--   0        0        0      531 2024-05-01 17:52:18.963014 edgegap_settings-1.2.0/edgegap_settings/_apm.py
--rw-r--r--   0        0        0      872 2024-05-01 17:52:18.963014 edgegap_settings-1.2.0/edgegap_settings/_base.py
--rw-r--r--   0        0        0      119 2024-05-01 17:52:18.963014 edgegap_settings-1.2.0/edgegap_settings/_configuration.py
--rw-r--r--   0        0        0     2998 2024-05-01 17:52:18.963014 edgegap_settings-1.2.0/edgegap_settings/_factory.py
--rw-r--r--   0        0        0      917 2024-05-01 17:52:18.967014 edgegap_settings-1.2.0/edgegap_settings/_fields.py
--rw-r--r--   0        0        0      427 2024-05-01 17:52:18.967014 edgegap_settings-1.2.0/edgegap_settings/_logstash.py
--rw-r--r--   0        0        0      741 2024-05-01 17:52:35.219413 edgegap_settings-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2925 1970-01-01 00:00:00.000000 edgegap_settings-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-02 18:20:19.995672 edgegap_settings-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2182 2024-05-02 18:20:19.995672 edgegap_settings-1.5.0/README.md
+-rw-r--r--   0        0        0       17 2024-05-02 18:20:19.995672 edgegap_settings-1.5.0/edgegap_settings/BUILD
+-rw-r--r--   0        0        0      359 2024-05-02 18:20:19.995672 edgegap_settings-1.5.0/edgegap_settings/__init__.py
+-rw-r--r--   0        0        0      531 2024-05-02 18:20:19.995672 edgegap_settings-1.5.0/edgegap_settings/_apm.py
+-rw-r--r--   0        0        0      872 2024-05-02 18:20:19.995672 edgegap_settings-1.5.0/edgegap_settings/_base.py
+-rw-r--r--   0        0        0      119 2024-05-02 18:20:19.995672 edgegap_settings-1.5.0/edgegap_settings/_configuration.py
+-rw-r--r--   0        0        0     2998 2024-05-02 18:20:19.995672 edgegap_settings-1.5.0/edgegap_settings/_factory.py
+-rw-r--r--   0        0        0      917 2024-05-02 18:20:19.995672 edgegap_settings-1.5.0/edgegap_settings/_fields.py
+-rw-r--r--   0        0        0      427 2024-05-02 18:20:19.995672 edgegap_settings-1.5.0/edgegap_settings/_logstash.py
+-rw-r--r--   0        0        0      741 2024-05-02 18:20:52.844507 edgegap_settings-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2925 1970-01-01 00:00:00.000000 edgegap_settings-1.5.0/PKG-INFO
```

### Comparing `edgegap_settings-1.2.0/LICENSE` & `edgegap_settings-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.2.0/README.md` & `edgegap_settings-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.2.0/edgegap_settings/_apm.py` & `edgegap_settings-1.5.0/edgegap_settings/_apm.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.2.0/edgegap_settings/_base.py` & `edgegap_settings-1.5.0/edgegap_settings/_base.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.2.0/edgegap_settings/_factory.py` & `edgegap_settings-1.5.0/edgegap_settings/_factory.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.2.0/edgegap_settings/_fields.py` & `edgegap_settings-1.5.0/edgegap_settings/_fields.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.2.0/pyproject.toml` & `edgegap_settings-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-settings"
-version = "1.2.0"
+version = "1.5.0"
 description = "The Edgegap Settings library includes various tools and helpers for interacting with Explicit Settings Models. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic-settings = "^2.2.1"
```

### Comparing `edgegap_settings-1.2.0/PKG-INFO` & `edgegap_settings-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-settings
-Version: 1.2.0
+Version: 1.5.0
 Summary: The Edgegap Settings library includes various tools and helpers for interacting with Explicit Settings Models. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

