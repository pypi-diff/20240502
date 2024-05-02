# Comparing `tmp/pytest_bec_e2e-2.9.5.tar.gz` & `tmp/pytest_bec_e2e-2.9.6.tar.gz`

## Comparing `pytest_bec_e2e-2.9.5.tar` & `pytest_bec_e2e-2.9.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_bec_e2e-2.9.5/pytest_bec_e2e/__init__.py
--rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 pytest_bec_e2e-2.9.5/pytest_bec_e2e/plugin.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 pytest_bec_e2e-2.9.5/.gitignore
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pytest_bec_e2e-2.9.5/pyproject.toml
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 pytest_bec_e2e-2.9.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_bec_e2e-2.9.6/pytest_bec_e2e/__init__.py
+-rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 pytest_bec_e2e-2.9.6/pytest_bec_e2e/plugin.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 pytest_bec_e2e-2.9.6/.gitignore
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pytest_bec_e2e-2.9.6/pyproject.toml
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 pytest_bec_e2e-2.9.6/PKG-INFO
```

### Comparing `pytest_bec_e2e-2.9.5/pytest_bec_e2e/plugin.py` & `pytest_bec_e2e-2.9.6/pytest_bec_e2e/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_bec_e2e-2.9.5/.gitignore` & `pytest_bec_e2e-2.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_bec_e2e-2.9.5/pyproject.toml` & `pytest_bec_e2e-2.9.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytest-bec-e2e"
-version = "2.9.5"
+version = "2.9.6"
 description = "BEC pytest plugin for end-to-end tests"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `pytest_bec_e2e-2.9.5/PKG-INFO` & `pytest_bec_e2e-2.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pytest-bec-e2e
-Version: 2.9.5
+Version: 2.9.6
 Summary: BEC pytest plugin for end-to-end tests
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Project-URL: Homepage, https://gitlab.psi.ch/bec/bec
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
```

