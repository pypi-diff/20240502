# Comparing `tmp/pytest_ruff-0.3.1.tar.gz` & `tmp/pytest_ruff-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_ruff-0.3.1.tar", max compression
+gzip compressed data, was "pytest_ruff-0.3.2.tar", max compression
```

## Comparing `pytest_ruff-0.3.1.tar` & `pytest_ruff-0.3.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1062 2024-03-10 12:49:29.749364 pytest_ruff-0.3.1/LICENSE
--rw-r--r--   0        0        0      628 2024-03-10 12:49:29.749364 pytest_ruff-0.3.1/README.md
--rw-r--r--   0        0        0     1562 2024-03-10 12:49:57.765150 pytest_ruff-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3575 2024-03-10 12:49:29.749364 pytest_ruff-0.3.1/pytest_ruff/__init__.py
--rw-r--r--   0        0        0     1113 2024-03-10 12:49:29.749364 pytest_ruff-0.3.1/pytest_ruff/_pytest_compat.py
--rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 pytest_ruff-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-02 06:45:11.103110 pytest_ruff-0.3.2/LICENSE
+-rw-r--r--   0        0        0      628 2024-05-02 06:45:11.103110 pytest_ruff-0.3.2/README.md
+-rw-r--r--   0        0        0     1562 2024-05-02 06:45:39.026935 pytest_ruff-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3728 2024-05-02 06:45:11.103110 pytest_ruff-0.3.2/pytest_ruff/__init__.py
+-rw-r--r--   0        0        0     1113 2024-05-02 06:45:11.103110 pytest_ruff-0.3.2/pytest_ruff/_pytest_compat.py
+-rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 pytest_ruff-0.3.2/PKG-INFO
```

### Comparing `pytest_ruff-0.3.1/LICENSE` & `pytest_ruff-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_ruff-0.3.1/README.md` & `pytest_ruff-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest_ruff-0.3.1/pyproject.toml` & `pytest_ruff-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-ruff"
-version = "0.3.1"
+version = "0.3.2"
 description = "pytest plugin to check ruff requirements."
 authors = ["Iuri de Silvio <iurisilvio@gmail.com>"]
 readme = "README.md"
 classifiers = [ "Development Status :: 4 - Beta", "Intended Audience :: Developers", "Operating System :: OS Independent", "Framework :: Pytest", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3 :: Only", "Topic :: Software Development :: Libraries :: Python Modules"]
 
 [tool.poetry.urls]
 Homepage = "https://github.com/businho/pytest-ruff"
```

### Comparing `pytest_ruff-0.3.1/pytest_ruff/__init__.py` & `pytest_ruff-0.3.2/pytest_ruff/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,14 +99,19 @@
     with Popen(command) as child:
         pass
 
     if child.returncode == 1:
         raise RuffError("File would be reformatted")
 
 
+def pytest_exception_interact(node, call, report):
+    if isinstance(call.excinfo.value, RuffError):
+        report.longrepr = str(call.excinfo.value)
+
+
 class RuffItem(pytest.Item):
     name = "ruff"
 
     def __init__(self, *k, **kwargs):
         super().__init__(*k, **kwargs)
         self.add_marker("ruff")
```

### Comparing `pytest_ruff-0.3.1/pytest_ruff/_pytest_compat.py` & `pytest_ruff-0.3.2/pytest_ruff/_pytest_compat.py`

 * *Files identical despite different names*

### Comparing `pytest_ruff-0.3.1/PKG-INFO` & `pytest_ruff-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-ruff
-Version: 0.3.1
+Version: 0.3.2
 Summary: pytest plugin to check ruff requirements.
 Author: Iuri de Silvio
 Author-email: iurisilvio@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

