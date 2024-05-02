# Comparing `tmp/bs_greenlight_cli-0.1.2.tar.gz` & `tmp/bs_greenlight_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_greenlight_cli-0.1.2.tar", max compression
+gzip compressed data, was "bs_greenlight_cli-0.2.0.tar", max compression
```

## Comparing `bs_greenlight_cli-0.1.2.tar` & `bs_greenlight_cli-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    18247 2024-05-01 15:05:22.782109 bs_greenlight_cli-0.1.2/glcli/cli.py
--rw-r--r--   0        0        0     4458 2024-05-01 15:05:22.782109 bs_greenlight_cli-0.1.2/glcli/environment.py
--rw-r--r--   0        0        0      623 2024-05-01 15:05:23.305157 bs_greenlight_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 bs_greenlight_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    18247 2024-04-25 10:56:10.795400 bs_greenlight_cli-0.2.0/glcli/cli.py
+-rw-r--r--   0        0        0     4458 2024-04-25 10:56:10.795400 bs_greenlight_cli-0.2.0/glcli/environment.py
+-rw-r--r--   0        0        0      623 2024-04-25 13:27:23.951438 bs_greenlight_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 bs_greenlight_cli-0.2.0/PKG-INFO
```

### Comparing `bs_greenlight_cli-0.1.2/glcli/cli.py` & `bs_greenlight_cli-0.2.0/glcli/cli.py`

 * *Files identical despite different names*

### Comparing `bs_greenlight_cli-0.1.2/glcli/environment.py` & `bs_greenlight_cli-0.2.0/glcli/environment.py`

 * *Files identical despite different names*

### Comparing `bs_greenlight_cli-0.1.2/pyproject.toml` & `bs_greenlight_cli-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bs-greenlight-cli"
-version = "0.1.2"
+version = "0.2.0"
 description = ""
 authors = ["Christian Decker <decker@blockstream.com>"]
 license = "MIT"
 
 packages = [
     { include = "glcli" },
 ]
```

### Comparing `bs_greenlight_cli-0.1.2/PKG-INFO` & `bs_greenlight_cli-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs-greenlight-cli
-Version: 0.1.2
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Christian Decker
 Author-email: decker@blockstream.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

