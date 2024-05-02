# Comparing `tmp/sql_unit_test-0.0.1.tar.gz` & `tmp/sql_unit_test-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_unit_test-0.0.1.tar", max compression
+gzip compressed data, was "sql_unit_test-0.1.0.tar", max compression
```

## Comparing `sql_unit_test-0.0.1.tar` & `sql_unit_test-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-04-27 20:28:20.598359 sql_unit_test-0.0.1/LICENSE
--rw-r--r--   0        0        0      946 2024-04-27 20:28:20.598359 sql_unit_test-0.0.1/README.md
--rw-r--r--   0        0        0      716 2024-04-27 20:28:20.598359 sql_unit_test-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       39 2024-04-27 20:28:20.602359 sql_unit_test-0.0.1/sql_unit_test/cli/__init__.py
--rw-r--r--   0        0        0      294 2024-04-27 20:28:20.602359 sql_unit_test-0.0.1/sql_unit_test/cli/commands.py
--rw-r--r--   0        0        0     3545 2024-04-27 20:28:20.602359 sql_unit_test-0.0.1/sql_unit_test/cli/outputs.py
--rw-r--r--   0        0        0      399 2024-04-27 20:28:20.602359 sql_unit_test-0.0.1/sql_unit_test/core/__init__.py
--rw-r--r--   0        0        0     2989 2024-04-27 20:28:20.602359 sql_unit_test-0.0.1/sql_unit_test/core/config.py
--rw-r--r--   0        0        0      834 2024-04-27 20:28:20.602359 sql_unit_test-0.0.1/sql_unit_test/core/config_manager.py
--rw-r--r--   0        0        0      444 2024-04-27 20:28:20.602359 sql_unit_test-0.0.1/sql_unit_test/core/connection.py
--rw-r--r--   0        0        0     1169 2024-04-27 20:28:20.602359 sql_unit_test-0.0.1/sql_unit_test/core/directory_check.py
--rw-r--r--   0        0        0     1214 2024-04-27 20:28:20.602359 sql_unit_test-0.0.1/sql_unit_test/core/initialize.py
--rw-r--r--   0        0        0      600 2024-04-27 20:28:20.602359 sql_unit_test-0.0.1/sql_unit_test/core/logger.py
--rw-r--r--   0        0        0     2152 2024-04-27 20:28:20.602359 sql_unit_test-0.0.1/sql_unit_test/core/run.py
--rw-r--r--   0        0        0     3060 2024-04-27 20:28:20.602359 sql_unit_test-0.0.1/sql_unit_test/core/run_test.py
--rw-r--r--   0        0        0      355 2024-04-27 20:28:20.602359 sql_unit_test-0.0.1/sql_unit_test/core/utils.py
--rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 sql_unit_test-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-02 18:26:09.413053 sql_unit_test-0.1.0/LICENSE
+-rw-r--r--   0        0        0      946 2024-05-02 18:26:09.413053 sql_unit_test-0.1.0/README.md
+-rw-r--r--   0        0        0      855 2024-05-02 18:26:09.413053 sql_unit_test-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-05-02 18:26:09.421053 sql_unit_test-0.1.0/sql_unit_test/cli/__init__.py
+-rw-r--r--   0        0        0      294 2024-05-02 18:26:09.421053 sql_unit_test-0.1.0/sql_unit_test/cli/commands.py
+-rw-r--r--   0        0        0     3545 2024-05-02 18:26:09.421053 sql_unit_test-0.1.0/sql_unit_test/cli/outputs.py
+-rw-r--r--   0        0        0      399 2024-05-02 18:26:09.421053 sql_unit_test-0.1.0/sql_unit_test/core/__init__.py
+-rw-r--r--   0        0        0     2989 2024-05-02 18:26:09.421053 sql_unit_test-0.1.0/sql_unit_test/core/config.py
+-rw-r--r--   0        0        0      834 2024-05-02 18:26:09.421053 sql_unit_test-0.1.0/sql_unit_test/core/config_manager.py
+-rw-r--r--   0        0        0      444 2024-05-02 18:26:09.421053 sql_unit_test-0.1.0/sql_unit_test/core/connection.py
+-rw-r--r--   0        0        0     1169 2024-05-02 18:26:09.421053 sql_unit_test-0.1.0/sql_unit_test/core/directory_check.py
+-rw-r--r--   0        0        0     1214 2024-05-02 18:26:09.421053 sql_unit_test-0.1.0/sql_unit_test/core/initialize.py
+-rw-r--r--   0        0        0      600 2024-05-02 18:26:09.421053 sql_unit_test-0.1.0/sql_unit_test/core/logger.py
+-rw-r--r--   0        0        0     2152 2024-05-02 18:26:09.421053 sql_unit_test-0.1.0/sql_unit_test/core/run.py
+-rw-r--r--   0        0        0     3075 2024-05-02 18:26:09.421053 sql_unit_test-0.1.0/sql_unit_test/core/run_test.py
+-rw-r--r--   0        0        0      721 2024-05-02 18:26:09.421053 sql_unit_test-0.1.0/sql_unit_test/core/utils.py
+-rw-r--r--   0        0        0     1678 1970-01-01 00:00:00.000000 sql_unit_test-0.1.0/PKG-INFO
```

### Comparing `sql_unit_test-0.0.1/LICENSE` & `sql_unit_test-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_unit_test-0.0.1/README.md` & `sql_unit_test-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sql_unit_test-0.0.1/pyproject.toml` & `sql_unit_test-0.1.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-unit-test"
-version = "0.0.1"
+version = "0.1.0"
 description = "A CLI tool for executing sql unit tests."
 authors = ["cohenj20 <cohenj20@sacredheart.edu>"]
 readme = "README.md"
 license = "MIT"
 include = [
     "LICENSE",
 ]
@@ -13,23 +13,29 @@
 python = "^3.10"
 colorama = "^0.4.6"
 click = "^8.1.7"
 pandas = "^2.2.1"
 pyodbc = "^5.1.0"
 sqlalchemy = "2.0.28"
 pyyaml = "^6.0.1"
-mkdocs = "^1.5.3"
-mkdocs-material-extensions = "^1.3.1"
-mkdocs-material = "^9.5.17"
-pytest = "^8.1.2"
 
 [tool.poetry.scripts]
 sql-unit-test = 'sql_unit_test.cli.commands:my_commands'
 
-
-
 [tool.poetry.group.dev.dependencies]
 commitizen = "^3.22.0"
+mkdocs = "^1.5.3"
+mkdocs-material-extensions = "^1.3.1"
+mkdocs-material = "^9.5.17"
+pytest = "^8.1.2"
+pytest-cov = "^5.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.commitizen]
+name = "cz_conventional_commits"
+version = "0.1.0"
+version_files = [
+    "pyproject.toml:version"
+]
```

### Comparing `sql_unit_test-0.0.1/sql_unit_test/cli/outputs.py` & `sql_unit_test-0.1.0/sql_unit_test/cli/outputs.py`

 * *Files identical despite different names*

### Comparing `sql_unit_test-0.0.1/sql_unit_test/core/config.py` & `sql_unit_test-0.1.0/sql_unit_test/core/config.py`

 * *Files identical despite different names*

### Comparing `sql_unit_test-0.0.1/sql_unit_test/core/config_manager.py` & `sql_unit_test-0.1.0/sql_unit_test/core/config_manager.py`

 * *Files identical despite different names*

### Comparing `sql_unit_test-0.0.1/sql_unit_test/core/directory_check.py` & `sql_unit_test-0.1.0/sql_unit_test/core/directory_check.py`

 * *Files identical despite different names*

### Comparing `sql_unit_test-0.0.1/sql_unit_test/core/initialize.py` & `sql_unit_test-0.1.0/sql_unit_test/core/initialize.py`

 * *Files identical despite different names*

### Comparing `sql_unit_test-0.0.1/sql_unit_test/core/logger.py` & `sql_unit_test-0.1.0/sql_unit_test/core/logger.py`

 * *Files identical despite different names*

### Comparing `sql_unit_test-0.0.1/sql_unit_test/core/run.py` & `sql_unit_test-0.1.0/sql_unit_test/core/run.py`

 * *Files identical despite different names*

### Comparing `sql_unit_test-0.0.1/sql_unit_test/core/run_test.py` & `sql_unit_test-0.1.0/sql_unit_test/core/run_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pandas as pd
 import logging
 import colorama
 import time
 import json
 import time
+import os
 
 from sql_unit_test.cli.outputs import report_failing_test_result, report_passing_test_result, report_test_sql_query_error
 from sql_unit_test.core.config import locate_root_dir
 from sql_unit_test.core.utils import parse_filename
 
 logger = logging.getLogger(__name__)
 
@@ -74,19 +75,19 @@
 
     logger.info('Successfully created failure file.')
     return failure_file_path
 
 def handle_test_result(test_result_df, test_duration, test_filename, test_file_path):
     if test_result_df.empty:
         logger.info('Sql unit test PASSED.')
-        report_passing_test_result(test_file_path=test_file_path, test_duration=test_duration)
+        report_passing_test_result(test_duration=test_duration)
         
     else:
         logger.info('Sql unit test FAILED.')
         failure_file_path = create_failure_file(test_results=test_result_df, test_filename=test_filename, test_duration=test_duration)
 
-        report_failing_test_result(test_file_path=test_file_path, failure_file_path=failure_file_path, test_duration=test_duration)
+        report_failing_test_result(test_file_path=os.path.normpath(test_file_path), failure_file_path=os.path.normpath(failure_file_path), test_duration=test_duration)
```

### Comparing `sql_unit_test-0.0.1/PKG-INFO` & `sql_unit_test-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 2.1
 Name: sql-unit-test
-Version: 0.0.1
+Version: 0.1.0
 Summary: A CLI tool for executing sql unit tests.
 License: MIT
 Author: cohenj20
 Author-email: cohenj20@sacredheart.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
-Requires-Dist: mkdocs (>=1.5.3,<2.0.0)
-Requires-Dist: mkdocs-material (>=9.5.17,<10.0.0)
-Requires-Dist: mkdocs-material-extensions (>=1.3.1,<2.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: pyodbc (>=5.1.0,<6.0.0)
-Requires-Dist: pytest (>=8.1.2,<9.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: sqlalchemy (==2.0.28)
 Description-Content-Type: text/markdown
 
 
 > [!IMPORTANT]
 > ***This site is currently under development*** . Please do not use it as a reference for finalized procedures, guides, or standards.
```

