# Comparing `tmp/pyathena-3.7.0.tar.gz` & `tmp/pyathena-3.8.0.tar.gz`

## Comparing `pyathena-3.7.0.tar` & `pyathena-3.8.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/__init__.py
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/async_cursor.py
--rw-r--r--   0        0        0    23825 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/common.py
--rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/connection.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/converter.py
--rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/cursor.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/error.py
--rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/formatter.py
--rw-r--r--   0        0        0    22930 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/py.typed
--rw-r--r--   0        0        0    23041 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/result_set.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/util.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/arrow/__init__.py
--rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/arrow/async_cursor.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/arrow/converter.py
--rw-r--r--   0        0        0     6854 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/arrow/cursor.py
--rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/arrow/result_set.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/arrow/util.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/fastparquet/__init__.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/fastparquet/util.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/filesystem/__init__.py
--rw-r--r--   0        0        0    20467 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/filesystem/s3.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/filesystem/s3_object.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/pandas/__init__.py
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/pandas/async_cursor.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/pandas/converter.py
--rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/pandas/cursor.py
--rw-r--r--   0        0        0    13467 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/pandas/result_set.py
--rw-r--r--   0        0        0    10297 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/pandas/util.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/spark/__init__.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/spark/async_cursor.py
--rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/spark/common.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/spark/cursor.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/sqlalchemy/arrow.py
--rw-r--r--   0        0        0    42007 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/sqlalchemy/base.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/sqlalchemy/pandas.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/sqlalchemy/requirements.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/sqlalchemy/rest.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/sqlalchemy/types.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyathena/sqlalchemy/util.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pyathena-3.7.0/.gitignore
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pyathena-3.7.0/LICENSE
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 pyathena-3.7.0/README.rst
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 pyathena-3.7.0/pyproject.toml
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 pyathena-3.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/__init__.py
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/async_cursor.py
+-rw-r--r--   0        0        0    23825 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/common.py
+-rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/connection.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/converter.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/cursor.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/error.py
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/formatter.py
+-rw-r--r--   0        0        0    22930 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/py.typed
+-rw-r--r--   0        0        0    23041 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/result_set.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/util.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/arrow/__init__.py
+-rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/arrow/async_cursor.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/arrow/converter.py
+-rw-r--r--   0        0        0     6854 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/arrow/cursor.py
+-rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/arrow/result_set.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/arrow/util.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/fastparquet/__init__.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/fastparquet/util.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/filesystem/__init__.py
+-rw-r--r--   0        0        0    33151 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/filesystem/s3.py
+-rw-r--r--   0        0        0    14350 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/filesystem/s3_object.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/pandas/__init__.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/pandas/async_cursor.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/pandas/converter.py
+-rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/pandas/cursor.py
+-rw-r--r--   0        0        0    13467 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/pandas/result_set.py
+-rw-r--r--   0        0        0    10297 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/pandas/util.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/spark/__init__.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/spark/async_cursor.py
+-rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/spark/common.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/spark/cursor.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/sqlalchemy/arrow.py
+-rw-r--r--   0        0        0    42007 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/sqlalchemy/base.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/sqlalchemy/pandas.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/sqlalchemy/rest.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/sqlalchemy/types.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/sqlalchemy/util.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pyathena-3.8.0/.gitignore
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pyathena-3.8.0/LICENSE
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 pyathena-3.8.0/README.rst
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 pyathena-3.8.0/PKG-INFO
```

### Comparing `pyathena-3.7.0/pyathena/__init__.py` & `pyathena-3.8.0/pyathena/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pyathena.error import *  # noqa
 
 if TYPE_CHECKING:
     from pyathena.connection import Connection, ConnectionCursor
     from pyathena.cursor import Cursor
 
-__version__ = "3.7.0"
+__version__ = "3.8.0"
 user_agent_extra: str = f"PyAthena/{__version__}"
 
 # Globals https://www.python.org/dev/peps/pep-0249/#globals
 apilevel: str = "2.0"
 threadsafety: int = 2
 paramstyle: str = "pyformat"
```

### Comparing `pyathena-3.7.0/pyathena/async_cursor.py` & `pyathena-3.8.0/pyathena/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/common.py` & `pyathena-3.8.0/pyathena/common.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/connection.py` & `pyathena-3.8.0/pyathena/connection.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/converter.py` & `pyathena-3.8.0/pyathena/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/cursor.py` & `pyathena-3.8.0/pyathena/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/error.py` & `pyathena-3.8.0/pyathena/error.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/formatter.py` & `pyathena-3.8.0/pyathena/formatter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/model.py` & `pyathena-3.8.0/pyathena/model.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/result_set.py` & `pyathena-3.8.0/pyathena/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/util.py` & `pyathena-3.8.0/pyathena/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/arrow/async_cursor.py` & `pyathena-3.8.0/pyathena/arrow/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/arrow/converter.py` & `pyathena-3.8.0/pyathena/arrow/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/arrow/cursor.py` & `pyathena-3.8.0/pyathena/arrow/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/arrow/result_set.py` & `pyathena-3.8.0/pyathena/arrow/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/arrow/util.py` & `pyathena-3.8.0/pyathena/arrow/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/fastparquet/util.py` & `pyathena-3.8.0/pyathena/fastparquet/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/pandas/async_cursor.py` & `pyathena-3.8.0/pyathena/pandas/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/pandas/converter.py` & `pyathena-3.8.0/pyathena/pandas/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/pandas/cursor.py` & `pyathena-3.8.0/pyathena/pandas/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/pandas/result_set.py` & `pyathena-3.8.0/pyathena/pandas/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/pandas/util.py` & `pyathena-3.8.0/pyathena/pandas/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/spark/async_cursor.py` & `pyathena-3.8.0/pyathena/spark/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/spark/common.py` & `pyathena-3.8.0/pyathena/spark/common.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/spark/cursor.py` & `pyathena-3.8.0/pyathena/spark/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/sqlalchemy/arrow.py` & `pyathena-3.8.0/pyathena/sqlalchemy/arrow.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/sqlalchemy/base.py` & `pyathena-3.8.0/pyathena/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/sqlalchemy/pandas.py` & `pyathena-3.8.0/pyathena/sqlalchemy/pandas.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/sqlalchemy/requirements.py` & `pyathena-3.8.0/pyathena/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyathena/sqlalchemy/types.py` & `pyathena-3.8.0/pyathena/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/LICENSE` & `pyathena-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/README.rst` & `pyathena-3.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyathena-3.7.0/pyproject.toml` & `pyathena-3.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,14 @@
 requirement_cls = "pyathena.sqlalchemy.requirements:Requirements"
 profile_file = "tests/sqlalchemy/profiles.txt"
 
 [tool.ruff]
 line-length = 100
 exclude = [
     ".venv",
-    "tests"
 ]
 target-version = "py38"
 
 [tool.ruff.lint]
 # https://docs.astral.sh/ruff/rules/
 select = [
     "E",  # pycodestyle errors
```

### Comparing `pyathena-3.7.0/PKG-INFO` & `pyathena-3.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: PyAthena
-Version: 3.7.0
+Version: 3.8.0
 Summary: Python DB API 2.0 (PEP 249) client for Amazon Athena
 Project-URL: homepage, https://github.com/laughingman7743/PyAthena/
 Project-URL: repository, https://github.com/laughingman7743/PyAthena/
 Author-email: laughingman7743 <laughingman7743@gmail.com>
 License: Copyright 2017 laughingman7743
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

