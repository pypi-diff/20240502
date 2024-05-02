# Comparing `tmp/capture_db_queries-1.0.1.tar.gz` & `tmp/capture_db_queries-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capture_db_queries-1.0.1.tar", last modified: Tue Apr 30 13:44:28 2024, max compression
+gzip compressed data, was "capture_db_queries-1.0.2.tar", last modified: Thu May  2 17:18:59 2024, max compression
```

## Comparing `capture_db_queries-1.0.1.tar` & `capture_db_queries-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:44:28.624721 capture_db_queries-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:44:28.620721 capture_db_queries-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:44:28.620721 capture_db_queries-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-04-30 13:44:28.624721 capture_db_queries-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:44:28.624721 capture_db_queries-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:44:28.620721 capture_db_queries-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:44:28.620721 capture_db_queries-1.0.1/src/capture_db_queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/src/capture_db_queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/src/capture_db_queries/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/src/capture_db_queries/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:44:28.624721 capture_db_queries-1.0.1/src/capture_db_queries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-04-30 13:44:28.000000 capture_db_queries-1.0.1/src/capture_db_queries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-30 13:44:28.000000 capture_db_queries-1.0.1/src/capture_db_queries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:44:28.000000 capture_db_queries-1.0.1/src/capture_db_queries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-30 13:44:28.000000 capture_db_queries-1.0.1/src/capture_db_queries.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-30 13:44:28.000000 capture_db_queries-1.0.1/src/capture_db_queries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 13:44:28.000000 capture_db_queries-1.0.1/src/capture_db_queries.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:44:28.624721 capture_db_queries-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-30 13:44:24.000000 capture_db_queries-1.0.1/tests/test_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:59.149221 capture_db_queries-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-02 17:18:54.000000 capture_db_queries-1.0.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:59.145221 capture_db_queries-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:59.145221 capture_db_queries-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-02 17:18:54.000000 capture_db_queries-1.0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-02 17:18:54.000000 capture_db_queries-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-02 17:18:54.000000 capture_db_queries-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-02 17:18:54.000000 capture_db_queries-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 17:18:54.000000 capture_db_queries-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10841 2024-05-02 17:18:59.149221 capture_db_queries-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-05-02 17:18:54.000000 capture_db_queries-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12173 2024-05-02 17:18:54.000000 capture_db_queries-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-02 17:18:59.149221 capture_db_queries-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:59.145221 capture_db_queries-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:59.145221 capture_db_queries-1.0.2/src/capture_db_queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:54.000000 capture_db_queries-1.0.2/src/capture_db_queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-05-02 17:18:54.000000 capture_db_queries-1.0.2/src/capture_db_queries/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-02 17:18:54.000000 capture_db_queries-1.0.2/src/capture_db_queries/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:59.149221 capture_db_queries-1.0.2/src/capture_db_queries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10841 2024-05-02 17:18:59.000000 capture_db_queries-1.0.2/src/capture_db_queries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-02 17:18:59.000000 capture_db_queries-1.0.2/src/capture_db_queries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:18:59.000000 capture_db_queries-1.0.2/src/capture_db_queries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-02 17:18:59.000000 capture_db_queries-1.0.2/src/capture_db_queries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-02 17:18:59.000000 capture_db_queries-1.0.2/src/capture_db_queries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 17:18:59.000000 capture_db_queries-1.0.2/src/capture_db_queries.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:59.149221 capture_db_queries-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:54.000000 capture_db_queries-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-02 17:18:54.000000 capture_db_queries-1.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-02 17:18:54.000000 capture_db_queries-1.0.2/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-02 17:18:54.000000 capture_db_queries-1.0.2/tests/test_decorators.py
```

### Comparing `capture_db_queries-1.0.1/.editorconfig` & `capture_db_queries-1.0.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `capture_db_queries-1.0.1/.github/workflows/publish-to-pypi.yml` & `capture_db_queries-1.0.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `capture_db_queries-1.0.1/.pre-commit-config.yaml` & `capture_db_queries-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `capture_db_queries-1.0.1/CONTRIBUTING.md` & `capture_db_queries-1.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `capture_db_queries-1.0.1/LICENSE` & `capture_db_queries-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `capture_db_queries-1.0.1/PKG-INFO` & `capture_db_queries-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: capture_db_queries
-Version: 1.0.1
+Version: 1.0.2
 Summary: Decorator for measuring the time and number of database queries
+Home-page: https://github.com/Friskes/capture-db-queries
+Author: Friskes
 Author-email: Friskes <friskesx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Friskes
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -21,17 +23,17 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Repository, https://github.com/Friskes/capture-db-queries
+Project-URL: Homepage, https://github.com/Friskes/capture-db-queries
 Project-URL: Changelog, https://github.com/Friskes/capture-db-queries/releases/
-Project-URL: Bug Reports, https://github.com/Friskes/capture-db-queries/issues
+Project-URL: Issues, https://github.com/Friskes/capture-db-queries/issues
 Keywords: Django,Database
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `capture_db_queries-1.0.1/README.md` & `capture_db_queries-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `capture_db_queries-1.0.1/pyproject.toml` & `capture_db_queries-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -54,17 +54,17 @@
     "pytest>=7.0.1",
     "mypy>=1.10.0",
     "pytest-cov>=5.0.0",
 ]
 
 
 [project.urls]
-"Repository" = "https://github.com/Friskes/capture-db-queries"
-"Changelog" = "https://github.com/Friskes/capture-db-queries/releases/"
-"Bug Reports" = "https://github.com/Friskes/capture-db-queries/issues"
+Homepage = "https://github.com/Friskes/capture-db-queries"
+Changelog = "https://github.com/Friskes/capture-db-queries/releases/"
+Issues = "https://github.com/Friskes/capture-db-queries/issues"
 
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=8"]
 build-backend = "setuptools.build_meta"
```

### Comparing `capture_db_queries-1.0.1/src/capture_db_queries/decorators.py` & `capture_db_queries-1.0.2/src/capture_db_queries/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     Median time one test is: Среднее время выполнения одного тестового замера
     """  # noqa: E501
 
     def _wrapper(func: DecoratedCallable) -> None:
         """"""
 
         @functools.wraps(func)
-        def spoof_func(*args: Any, **kwargs: Any) -> Any:
+        def spoof_func(*args: Any, **kwargs: Any) -> None:
             """"""
             force_debug_cursor = connection.force_debug_cursor
             connection.force_debug_cursor = True
             # Run any initialization queries if needed so that they won't be
             # included as part of the count.
             connection.ensure_connection()
             initial_queries = len(connection.queries_log)
```

### Comparing `capture_db_queries-1.0.1/src/capture_db_queries.egg-info/PKG-INFO` & `capture_db_queries-1.0.2/src/capture_db_queries.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: capture_db_queries
-Version: 1.0.1
+Version: 1.0.2
 Summary: Decorator for measuring the time and number of database queries
+Home-page: https://github.com/Friskes/capture-db-queries
+Author: Friskes
 Author-email: Friskes <friskesx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Friskes
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -21,17 +23,17 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Repository, https://github.com/Friskes/capture-db-queries
+Project-URL: Homepage, https://github.com/Friskes/capture-db-queries
 Project-URL: Changelog, https://github.com/Friskes/capture-db-queries/releases/
-Project-URL: Bug Reports, https://github.com/Friskes/capture-db-queries/issues
+Project-URL: Issues, https://github.com/Friskes/capture-db-queries/issues
 Keywords: Django,Database
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `capture_db_queries-1.0.1/src/capture_db_queries.egg-info/SOURCES.txt` & `capture_db_queries-1.0.2/src/capture_db_queries.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .editorconfig
 .gitignore
 .pre-commit-config.yaml
 CONTRIBUTING.md
 LICENSE
 README.md
 pyproject.toml
+setup.cfg
 .github/workflows/publish-to-pypi.yml
 src/capture_db_queries/__init__.py
 src/capture_db_queries/decorators.py
 src/capture_db_queries/types.py
 src/capture_db_queries.egg-info/PKG-INFO
 src/capture_db_queries.egg-info/SOURCES.txt
 src/capture_db_queries.egg-info/dependency_links.txt
```

### Comparing `capture_db_queries-1.0.1/tests/conftest.py` & `capture_db_queries-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `capture_db_queries-1.0.1/tests/test_decorators.py` & `capture_db_queries-1.0.2/tests/test_decorators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import re
 from io import StringIO
 
 import pytest
 from django.utils import timezone
 from src.capture_db_queries.decorators import ExtCaptureQueriesContext, capture_queries
 
 from tests.models import Article, Reporter
 
+ANYNUM = r'0.0[0-9]+'
+
 
 # python -m pip install .
 # pytest -s -v ./tests
 @pytest.mark.django_db(transaction=True)
 def test_capture_queries(intercept_output: StringIO) -> None:
     """Обязательно должен быть передан аргумент -s при запуске pytest, для вывода output"""
 
@@ -19,20 +22,60 @@
         Article.objects.create(
             pub_date=timezone.now().date(),
             headline='headline',
             content='content',
             reporter=reporter,
         )
 
-    value = intercept_output.getvalue()
-    assert value[:72] == 'Tests count: 100  |  Total queries count: 200  |  Total execution time: '
-    # assert float(value[72:76]) in [x / 100.0 for x in range(1, 4)]
-    assert value[76:107] == 's  |  Median time one test is: '
-    # assert float(value[107:112]) in [x / 1000.0 for x in range(1)]
-    assert value[112:114] == 's\n'
+    output = intercept_output.getvalue()
+
+    assert re.match(
+        f'Tests count: 100  |  Total queries count: 200  |  Total execution time: {ANYNUM}s  |  Median time one test is: {ANYNUM}s\n',  # noqa: E501
+        output,
+    ), 'incorrect output'
+
+
+@pytest.mark.django_db(transaction=True)
+def test_capture_queries_with_advanced_verb_and_queries(intercept_output: StringIO) -> None:
+    """Обязательно должен быть передан аргумент -s при запуске pytest, для вывода output"""
+
+    date_now = timezone.now().date()
+
+    @capture_queries(number_runs=2, advanced_verb=True, queries=True)
+    def _() -> None:
+        reporter = Reporter.objects.create(full_name='full_name')
+        Article.objects.create(
+            pub_date=date_now,
+            headline='headline',
+            content='content',
+            reporter=reporter,
+        )
+
+    output = intercept_output.getvalue()
+    result_outputs = [x for x in output.split('\n') if x != '']
+
+    correct_outputs = [
+        f'Test №1 | Queries count: 2 | Execution time: {ANYNUM}s',
+        f'Test №2 | Queries count: 2 | Execution time: {ANYNUM}s',
+        '---SQL query---',
+        '---SQL query---',
+        '---SQL query---',
+        '---SQL query---',
+        f'Tests count: 2  |  Total queries count: 4  |  Total execution time: {ANYNUM}s  |  Median time one test is: {ANYNUM}s',  # noqa: E501
+    ]
+
+    assert len(result_outputs) == len(correct_outputs)
+
+    for result_output, correct_output in zip(result_outputs, correct_outputs):  # noqa: B905
+        if result_output.startswith("{'sql':"):
+            continue
+        assert re.match(
+            correct_output,
+            result_output,
+        ), 'incorrect output'
 
 
 @pytest.mark.django_db(transaction=True)
 def test_ext_capture_queries_context(intercept_output: StringIO) -> None:
     """Обязательно должен быть передан аргумент -s при запуске pytest, для вывода output"""
 
     with ExtCaptureQueriesContext() as ctx:
@@ -40,11 +83,13 @@
         Article.objects.create(
             pub_date=timezone.now().date(),
             headline='headline',
             content='content',
             reporter=reporter,
         )
 
-    value = intercept_output.getvalue()
-    assert value[:37] == 'Queries count: 2  |  Execution time: '
-    # assert float(value[37:42]) in [x / 1000.0 for x in range(2)]
-    assert value[42:43] == 's'
+    output = intercept_output.getvalue()
+
+    assert re.match(
+        f'Queries count: 2  |  Execution time: {ANYNUM}s',
+        output,
+    ), 'incorrect output'
```

