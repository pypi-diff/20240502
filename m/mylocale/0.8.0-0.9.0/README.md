# Comparing `tmp/mylocale-0.8.0.tar.gz` & `tmp/mylocale-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mylocale-0.8.0.tar", max compression
+gzip compressed data, was "mylocale-0.9.0.tar", max compression
```

## Comparing `mylocale-0.8.0.tar` & `mylocale-0.9.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2024-03-10 18:35:20.890725 mylocale-0.8.0/LICENSE
--rw-r--r--   0        0        0      168 2024-03-31 21:13:36.582821 mylocale-0.8.0/README.md
--rw-r--r--   0        0        0      433 2024-03-31 21:40:48.899977 mylocale-0.8.0/mylocale/TR.py
--rw-r--r--   0        0        0       17 2024-03-31 21:42:12.824819 mylocale-0.8.0/mylocale/__init__.py
--rw-r--r--   0        0        0      510 2024-03-31 21:42:25.808949 mylocale-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 mylocale-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-10 18:35:20.890725 mylocale-0.9.0/LICENSE
+-rw-r--r--   0        0        0      168 2024-03-31 21:13:36.582821 mylocale-0.9.0/README.md
+-rw-r--r--   0        0        0      433 2024-03-31 21:40:48.899977 mylocale-0.9.0/mylocale/TR.py
+-rw-r--r--   0        0        0        0 2024-03-31 21:49:27.900980 mylocale-0.9.0/mylocale/__init__.py
+-rw-r--r--   0        0        0      510 2024-03-31 21:49:47.653167 mylocale-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 mylocale-0.9.0/PKG-INFO
```

### Comparing `mylocale-0.8.0/LICENSE` & `mylocale-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mylocale-0.8.0/PKG-INFO` & `mylocale-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mylocale
-Version: 0.8.0
+Version: 0.9.0
 Summary: A simple python library for simple localisation wit CSV files.
 Home-page: https://github.com/tct123/mylocale
 License: MIT
 Author: tct123
 Author-email: 42028373+tct123@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

