# Comparing `tmp/transformers_js_py-0.8.1.tar.gz` & `tmp/transformers_js_py-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers_js_py-0.8.1.tar", max compression
+gzip compressed data, was "transformers_js_py-0.9.0.tar", max compression
```

## Comparing `transformers_js_py-0.8.1.tar` & `transformers_js_py-0.9.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11357 2024-02-26 07:18:57.270000 transformers_js_py-0.8.1/LICENSE
--rw-r--r--   0        0        0    13161 2024-02-26 07:18:57.270000 transformers_js_py-0.8.1/README.md
--rw-r--r--   0        0        0      837 2024-02-26 07:18:57.278000 transformers_js_py-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      265 2024-02-26 07:18:57.278000 transformers_js_py-0.8.1/transformers_js/__init__.py
--rw-r--r--   0        0        0      116 2024-02-26 07:18:57.278000 transformers_js_py-0.8.1/transformers_js_py/__init__.py
--rw-r--r--   0        0        0     6571 2024-02-26 07:18:57.278000 transformers_js_py-0.8.1/transformers_js_py/proxies.py
--rw-r--r--   0        0        0     1995 2024-02-26 07:18:57.278000 transformers_js_py-0.8.1/transformers_js_py/url.py
--rw-r--r--   0        0        0    13787 1970-01-01 00:00:00.000000 transformers_js_py-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-26 11:18:17.865929 transformers_js_py-0.9.0/LICENSE
+-rw-r--r--   0        0        0    13161 2024-02-26 11:18:17.865929 transformers_js_py-0.9.0/README.md
+-rw-r--r--   0        0        0      837 2024-02-26 11:18:17.873929 transformers_js_py-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      265 2024-02-26 11:18:17.873929 transformers_js_py-0.9.0/transformers_js/__init__.py
+-rw-r--r--   0        0        0      160 2024-02-26 11:18:17.873929 transformers_js_py-0.9.0/transformers_js_py/__init__.py
+-rw-r--r--   0        0        0     1502 2024-02-26 11:18:17.873929 transformers_js_py-0.9.0/transformers_js_py/audio.py
+-rw-r--r--   0        0        0     6571 2024-02-26 11:18:17.873929 transformers_js_py-0.9.0/transformers_js_py/proxies.py
+-rw-r--r--   0        0        0     1995 2024-02-26 11:18:17.873929 transformers_js_py-0.9.0/transformers_js_py/url.py
+-rw-r--r--   0        0        0    13787 1970-01-01 00:00:00.000000 transformers_js_py-0.9.0/PKG-INFO
```

### Comparing `transformers_js_py-0.8.1/LICENSE` & `transformers_js_py-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `transformers_js_py-0.8.1/README.md` & `transformers_js_py-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `transformers_js_py-0.8.1/pyproject.toml` & `transformers_js_py-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "transformers-js-py"
-version = "0.8.1"
+version = "0.9.0"
 description = ""
 authors = ["Yuichiro Tachibana (Tsuchiya) <t.yic.yt@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     {include = "transformers_js_py"},
     {include = "transformers_js"},
```

### Comparing `transformers_js_py-0.8.1/transformers_js_py/proxies.py` & `transformers_js_py-0.9.0/transformers_js_py/proxies.py`

 * *Files identical despite different names*

### Comparing `transformers_js_py-0.8.1/transformers_js_py/url.py` & `transformers_js_py-0.9.0/transformers_js_py/url.py`

 * *Files identical despite different names*

### Comparing `transformers_js_py-0.8.1/PKG-INFO` & `transformers_js_py-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers-js-py
-Version: 0.8.1
+Version: 0.9.0
 Summary: 
 Home-page: https://github.com/whitphx/transformers.js.py
 License: Apache-2.0
 Author: Yuichiro Tachibana (Tsuchiya)
 Author-email: t.yic.yt@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

