# Comparing `tmp/midori-1.0.1.tar.gz` & `tmp/midori-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midori-1.0.1.tar", max compression
+gzip compressed data, was "midori-1.0.2.tar", max compression
```

## Comparing `midori-1.0.1.tar` & `midori-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6670 2024-05-02 20:25:29.117017 midori-1.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-02 20:25:29.121017 midori-1.0.1/midori/__init__.py
--rw-r--r--   0        0        0     4640 2024-05-02 20:25:29.121017 midori-1.0.1/midori/core.py
--rw-r--r--   0        0        0     1886 2024-05-02 20:25:29.121017 midori-1.0.1/midori/plugins/base.py
--rw-r--r--   0        0        0      928 2024-05-02 20:25:29.121017 midori-1.0.1/midori/plugins/example_plugins.py
--rw-r--r--   0        0        0     5473 2024-05-02 20:25:29.121017 midori-1.0.1/midori/plugins/helpers.py
--rw-r--r--   0        0        0      484 2024-05-02 20:25:29.121017 midori-1.0.1/midori/treatments_helper.py
--rw-r--r--   0        0        0      425 2024-05-02 20:25:29.121017 midori-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     7059 1970-01-01 00:00:00.000000 midori-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6670 2024-05-02 20:35:59.033413 midori-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 20:35:59.037413 midori-1.0.2/midori/__init__.py
+-rw-r--r--   0        0        0     4640 2024-05-02 20:35:59.037413 midori-1.0.2/midori/core.py
+-rw-r--r--   0        0        0     1886 2024-05-02 20:35:59.037413 midori-1.0.2/midori/plugins/base.py
+-rw-r--r--   0        0        0      928 2024-05-02 20:35:59.037413 midori-1.0.2/midori/plugins/example_plugins.py
+-rw-r--r--   0        0        0     5473 2024-05-02 20:35:59.037413 midori-1.0.2/midori/plugins/helpers.py
+-rw-r--r--   0        0        0      484 2024-05-02 20:35:59.037413 midori-1.0.2/midori/treatments_helper.py
+-rw-r--r--   0        0        0      425 2024-05-02 20:35:59.037413 midori-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7059 1970-01-01 00:00:00.000000 midori-1.0.2/PKG-INFO
```

### Comparing `midori-1.0.1/README.md` & `midori-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `midori-1.0.1/midori/core.py` & `midori-1.0.2/midori/core.py`

 * *Files identical despite different names*

### Comparing `midori-1.0.1/midori/plugins/base.py` & `midori-1.0.2/midori/plugins/base.py`

 * *Files identical despite different names*

### Comparing `midori-1.0.1/midori/plugins/example_plugins.py` & `midori-1.0.2/midori/plugins/example_plugins.py`

 * *Files identical despite different names*

### Comparing `midori-1.0.1/midori/plugins/helpers.py` & `midori-1.0.2/midori/plugins/helpers.py`

 * *Files identical despite different names*

### Comparing `midori-1.0.1/PKG-INFO` & `midori-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midori
-Version: 1.0.1
+Version: 1.0.2
 Summary: 🍃 streamline remote software engineering experiments
 Author: Xingwen Xiao
 Author-email: xingwen.xiao@student.uva.nl
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: paramiko (>=3.4.0,<4.0.0)
```

