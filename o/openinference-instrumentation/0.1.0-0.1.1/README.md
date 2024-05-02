# Comparing `tmp/openinference_instrumentation-0.1.0.tar.gz` & `tmp/openinference_instrumentation-0.1.1.tar.gz`

## Comparing `openinference_instrumentation-0.1.0.tar` & `openinference_instrumentation-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.0/src/openinference/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.0/src/openinference/instrumentation/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.0/src/openinference/instrumentation/version.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.0/tests/test_suppress_tracing.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.0/.gitignore
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.0/README.md
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.1/src/openinference/instrumentation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.1/src/openinference/instrumentation/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.1/src/openinference/instrumentation/version.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.1/tests/test_suppress_tracing.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.1/.gitignore
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.1/LICENSE
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.1/README.md
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.1/PKG-INFO
```

### Comparing `openinference_instrumentation-0.1.0/src/openinference/instrumentation/__init__.py` & `openinference_instrumentation-0.1.1/src/openinference/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation-0.1.0/tests/test_suppress_tracing.py` & `openinference_instrumentation-0.1.1/tests/test_suppress_tracing.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation-0.1.0/pyproject.toml` & `openinference_instrumentation-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation-0.1.0/PKG-INFO` & `openinference_instrumentation-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.3
 Name: openinference-instrumentation
-Version: 0.1.0
+Version: 0.1.1
 Summary: OpenInference instrumentation utilities
 Project-URL: Homepage, https://github.com/Arize-ai/openinference/tree/main/python/openinference-instrumentation
 Author-email: OpenInference Authors <oss@arize.com>
 License-Expression: Apache-2.0
+License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

