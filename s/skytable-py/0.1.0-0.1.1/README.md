# Comparing `tmp/skytable_py-0.1.0.tar.gz` & `tmp/skytable_py-0.1.1.tar.gz`

## Comparing `skytable_py-0.1.0.tar` & `skytable_py-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 skytable_py-0.1.0/run_tests.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 skytable_py-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 skytable_py-0.1.0/src/skytable_py/__init__.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 skytable_py-0.1.0/src/skytable_py/config.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 skytable_py-0.1.0/src/skytable_py/connection.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 skytable_py-0.1.0/src/skytable_py/exception.py
--rw-r--r--   0        0        0     8474 2020-02-02 00:00:00.000000 skytable_py-0.1.0/src/skytable_py/protocol.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 skytable_py-0.1.0/src/skytable_py/query.py
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 skytable_py-0.1.0/src/skytable_py/response.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 skytable_py-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 skytable_py-0.1.0/tests/test_config.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 skytable_py-0.1.0/tests/test_encoding.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 skytable_py-0.1.0/tests/test_protocol.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 skytable_py-0.1.0/tests/test_query.py
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 skytable_py-0.1.0/tests/test_response.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 skytable_py-0.1.0/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 skytable_py-0.1.0/LICENSE
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 skytable_py-0.1.0/README.md
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 skytable_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 skytable_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 skytable_py-0.1.1/run_tests.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 skytable_py-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 skytable_py-0.1.1/src/skytable_py/__init__.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 skytable_py-0.1.1/src/skytable_py/config.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 skytable_py-0.1.1/src/skytable_py/connection.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 skytable_py-0.1.1/src/skytable_py/exception.py
+-rw-r--r--   0        0        0     8474 2020-02-02 00:00:00.000000 skytable_py-0.1.1/src/skytable_py/protocol.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 skytable_py-0.1.1/src/skytable_py/query.py
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 skytable_py-0.1.1/src/skytable_py/response.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 skytable_py-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 skytable_py-0.1.1/tests/test_config.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 skytable_py-0.1.1/tests/test_encoding.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 skytable_py-0.1.1/tests/test_protocol.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 skytable_py-0.1.1/tests/test_query.py
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 skytable_py-0.1.1/tests/test_response.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 skytable_py-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 skytable_py-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 skytable_py-0.1.1/README.md
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 skytable_py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 skytable_py-0.1.1/PKG-INFO
```

### Comparing `skytable_py-0.1.0/run_tests.py` & `skytable_py-0.1.1/run_tests.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.0/.github/workflows/test.yml` & `skytable_py-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.0/src/skytable_py/__init__.py` & `skytable_py-0.1.1/src/skytable_py/__init__.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.0/src/skytable_py/config.py` & `skytable_py-0.1.1/src/skytable_py/config.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.0/src/skytable_py/connection.py` & `skytable_py-0.1.1/src/skytable_py/connection.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.0/src/skytable_py/exception.py` & `skytable_py-0.1.1/src/skytable_py/exception.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.0/src/skytable_py/protocol.py` & `skytable_py-0.1.1/src/skytable_py/protocol.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.0/src/skytable_py/query.py` & `skytable_py-0.1.1/src/skytable_py/query.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.0/src/skytable_py/response.py` & `skytable_py-0.1.1/src/skytable_py/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,20 +112,20 @@
     def float(self) -> Union[None, float]:
         if isinstance(self.repr, (Float32, Float64)):
             return self.repr.inner
         return None
 
     def string(self) -> Union[None, str]:
         if isinstance(self.repr, str):
-            return self.repr.inner
+            return self.repr
         return None
 
     def binary(self) -> Union[None, bytes]:
         if isinstance(self.repr, bytes):
-            return self.repr.inner
+            return self.repr
         return None
 
     def list(self) -> Union[None, list]:
         if isinstance(self.repr, list):
             return self.repr
         return None
```

### Comparing `skytable_py-0.1.0/tests/__init__.py` & `skytable_py-0.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.0/tests/test_config.py` & `skytable_py-0.1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.0/tests/test_encoding.py` & `skytable_py-0.1.1/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.0/tests/test_protocol.py` & `skytable_py-0.1.1/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.0/tests/test_query.py` & `skytable_py-0.1.1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.0/tests/test_response.py` & `skytable_py-0.1.1/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.0/LICENSE` & `skytable_py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.0/pyproject.toml` & `skytable_py-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "skytable-py"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{ name = "Sayan Nandan", email = "nandansayan@outlook.com" }]
 description = "Official Skytable client library for Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

