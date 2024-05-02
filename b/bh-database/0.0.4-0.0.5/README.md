# Comparing `tmp/bh-database-0.0.4.tar.gz` & `tmp/bh_database-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bh-database-0.0.4.tar", last modified: Thu May 11 01:27:00 2023, max compression
+gzip compressed data, was "bh_database-0.0.5.tar", last modified: Thu May  2 04:13:53 2024, max compression
```

## Comparing `bh-database-0.0.4.tar` & `bh_database-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 01:27:00.880742 bh-database-0.0.4/
--rw-rw-rw-   0        0        0     2484 2023-05-11 01:27:00.879744 bh-database-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1858 2023-01-25 03:51:11.000000 bh-database-0.0.4/README.md
--rw-rw-rw-   0        0        0     1033 2023-05-11 01:19:54.000000 bh-database-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 01:27:00.880742 bh-database-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-11 01:27:00.834746 bh-database-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 01:27:00.841743 bh-database-0.0.4/src/bh_database/
--rw-rw-rw-   0        0        0       90 2023-05-11 01:18:26.000000 bh-database-0.0.4/src/bh_database/__init__.py
--rw-rw-rw-   0        0        0    23937 2023-05-11 01:11:19.000000 bh-database-0.0.4/src/bh_database/base_table.py
--rw-rw-rw-   0        0        0     2239 2023-01-25 03:51:11.000000 bh-database-0.0.4/src/bh_database/constant.py
--rw-rw-rw-   0        0        0    18162 2023-05-11 00:51:04.000000 bh-database-0.0.4/src/bh_database/core.py
--rw-rw-rw-   0        0        0     5120 2023-01-25 03:51:11.000000 bh-database-0.0.4/src/bh_database/paginator.py
-drwxrwxrwx   0        0        0        0 2023-05-11 01:27:00.862740 bh-database-0.0.4/src/bh_database.egg-info/
--rw-rw-rw-   0        0        0     2484 2023-05-11 01:27:00.000000 bh-database-0.0.4/src/bh_database.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-05-11 01:27:00.000000 bh-database-0.0.4/src/bh_database.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 01:27:00.000000 bh-database-0.0.4/src/bh_database.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      198 2023-05-11 01:27:00.000000 bh-database-0.0.4/src/bh_database.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-11 01:27:00.000000 bh-database-0.0.4/src/bh_database.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-11 01:27:00.878742 bh-database-0.0.4/tests/
--rw-rw-rw-   0        0        0     5782 2023-01-25 03:51:11.000000 bh-database-0.0.4/tests/test_01_core_database_postgresql.py
--rw-rw-rw-   0        0        0     5682 2023-01-25 03:51:11.000000 bh-database-0.0.4/tests/test_02_core_database_mysql.py
--rw-rw-rw-   0        0        0     3956 2023-01-25 03:51:11.000000 bh-database-0.0.4/tests/test_05_core_basesqlalchemy_postgresql.py
--rw-rw-rw-   0        0        0     3634 2023-01-25 03:51:11.000000 bh-database-0.0.4/tests/test_06_core_basesqlalchemy_mysql.py
--rw-rw-rw-   0        0        0     3551 2023-05-10 03:56:40.000000 bh-database-0.0.4/tests/test_11_paginator_postgresql.py
--rw-rw-rw-   0        0        0     3466 2023-05-10 03:56:45.000000 bh-database-0.0.4/tests/test_12_paginator_mysql.py
--rw-rw-rw-   0        0        0     7571 2023-05-11 01:13:14.000000 bh-database-0.0.4/tests/test_15_base_table_postgresql.py
--rw-rw-rw-   0        0        0     7041 2023-05-11 01:06:29.000000 bh-database-0.0.4/tests/test_16_base_table_mysql.py
--rw-rw-rw-   0        0        0     1651 2023-01-25 03:51:11.000000 bh-database-0.0.4/tests/test_17_base_table_methods.py
--rw-rw-rw-   0        0        0     1616 2023-01-25 03:51:11.000000 bh-database-0.0.4/tests/test_20_base_table_dunder.py
--rw-rw-rw-   0        0        0    19413 2023-05-10 10:35:40.000000 bh-database-0.0.4/tests/test_25_base_table_crud_methods_postgresql.py
--rw-rw-rw-   0        0        0    19290 2023-05-10 10:38:52.000000 bh-database-0.0.4/tests/test_26_base_table_crud_methods_mysql.py
--rw-rw-rw-   0        0        0     4496 2023-05-10 03:58:11.000000 bh-database-0.0.4/tests/test_30_base_table_exception_postgresql.py
--rw-rw-rw-   0        0        0     4427 2023-05-10 03:57:49.000000 bh-database-0.0.4/tests/test_31_base_table_exception_mysql.py
+drwxrwxrwx   0        0        0        0 2024-05-02 04:13:53.049619 bh_database-0.0.5/
+-rw-rw-rw-   0        0        0     2981 2024-05-02 04:13:53.048615 bh_database-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1858 2023-01-25 03:51:11.000000 bh_database-0.0.5/README.md
+-rw-rw-rw-   0        0        0     1032 2024-05-02 04:10:19.000000 bh_database-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-02 04:13:53.049619 bh_database-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-02 04:13:53.018616 bh_database-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-02 04:13:53.025616 bh_database-0.0.5/src/bh_database/
+-rw-rw-rw-   0        0        0       90 2023-05-11 01:18:26.000000 bh_database-0.0.5/src/bh_database/__init__.py
+-rw-rw-rw-   0        0        0    23937 2023-05-11 01:11:19.000000 bh_database-0.0.5/src/bh_database/base_table.py
+-rw-rw-rw-   0        0        0     2239 2023-01-25 03:51:11.000000 bh_database-0.0.5/src/bh_database/constant.py
+-rw-rw-rw-   0        0        0    18987 2024-05-02 04:07:47.000000 bh_database-0.0.5/src/bh_database/core.py
+-rw-rw-rw-   0        0        0     5120 2023-01-25 03:51:11.000000 bh_database-0.0.5/src/bh_database/paginator.py
+drwxrwxrwx   0        0        0        0 2024-05-02 04:13:53.047617 bh_database-0.0.5/src/bh_database.egg-info/
+-rw-rw-rw-   0        0        0     2981 2024-05-02 04:13:52.000000 bh_database-0.0.5/src/bh_database.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2024-05-02 04:13:53.000000 bh_database-0.0.5/src/bh_database.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 04:13:52.000000 bh_database-0.0.5/src/bh_database.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-05-02 04:13:52.000000 bh_database-0.0.5/src/bh_database.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-02 04:13:52.000000 bh_database-0.0.5/src/bh_database.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 04:13:53.046615 bh_database-0.0.5/tests/
+-rw-rw-rw-   0        0        0     5782 2023-01-25 03:51:11.000000 bh_database-0.0.5/tests/test_01_core_database_postgresql.py
+-rw-rw-rw-   0        0        0     5682 2023-01-25 03:51:11.000000 bh_database-0.0.5/tests/test_02_core_database_mysql.py
+-rw-rw-rw-   0        0        0     3956 2023-01-25 03:51:11.000000 bh_database-0.0.5/tests/test_05_core_basesqlalchemy_postgresql.py
+-rw-rw-rw-   0        0        0     3634 2023-01-25 03:51:11.000000 bh_database-0.0.5/tests/test_06_core_basesqlalchemy_mysql.py
+-rw-rw-rw-   0        0        0     3551 2023-05-10 03:56:40.000000 bh_database-0.0.5/tests/test_11_paginator_postgresql.py
+-rw-rw-rw-   0        0        0     3466 2023-05-11 02:17:26.000000 bh_database-0.0.5/tests/test_12_paginator_mysql.py
+-rw-rw-rw-   0        0        0     7571 2023-05-11 02:16:44.000000 bh_database-0.0.5/tests/test_15_base_table_postgresql.py
+-rw-rw-rw-   0        0        0     7041 2023-05-11 02:17:26.000000 bh_database-0.0.5/tests/test_16_base_table_mysql.py
+-rw-rw-rw-   0        0        0     1651 2023-01-25 03:51:11.000000 bh_database-0.0.5/tests/test_17_base_table_methods.py
+-rw-rw-rw-   0        0        0     1616 2023-01-25 03:51:11.000000 bh_database-0.0.5/tests/test_20_base_table_dunder.py
+-rw-rw-rw-   0        0        0    19413 2023-05-11 02:16:44.000000 bh_database-0.0.5/tests/test_25_base_table_crud_methods_postgresql.py
+-rw-rw-rw-   0        0        0    19290 2024-04-11 01:41:30.000000 bh_database-0.0.5/tests/test_26_base_table_crud_methods_mysql.py
+-rw-rw-rw-   0        0        0     4496 2023-05-10 03:58:11.000000 bh_database-0.0.5/tests/test_30_base_table_exception_postgresql.py
+-rw-rw-rw-   0        0        0     4427 2024-04-11 01:41:30.000000 bh_database-0.0.5/tests/test_31_base_table_exception_mysql.py
```

### Comparing `bh-database-0.0.4/PKG-INFO` & `bh_database-0.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: bh-database
-Version: 0.0.4
-Summary: Database wrapper classes for SQLAlchemy.
-Author-email: Van Be Hai Nguyen <behai_nguyen@hotmail.com>
-Project-URL: repository, https://github.com/behai-nguyen/bh_database
-Project-URL: documentation, https://bh-database.readthedocs.io/
-Keywords: SQLAlchemy,database,wrapper
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: builds
-Provides-Extra: docs
-
 # bh_database
 
 Database wrapper classes for SQLAlchemy.
 
 ## Pip installation
 
 ```
@@ -67,8 +50,8 @@
 
 ## Documentation
 
 [Full documentation](https://bh-database.readthedocs.io/)
 
 ## License
 
-[ MIT license ](http://www.opensource.org/licenses/mit-license.php)
+[ MIT license ](http://www.opensource.org/licenses/mit-license.php)
```

### Comparing `bh-database-0.0.4/README.md` & `bh_database-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.1
+Name: bh-database
+Version: 0.0.5
+Summary: Database wrapper classes for SQLAlchemy.
+Author-email: Van Be Hai Nguyen <behai_nguyen@hotmail.com>
+Project-URL: repository, https://github.com/behai-nguyen/bh_database
+Project-URL: documentation, https://bh-database.readthedocs.io/
+Keywords: SQLAlchemy,database,wrapper
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Requires-Dist: tomli; python_version >= "3.10"
+Requires-Dist: SQLAlchemy
+Requires-Dist: psycopg2-binary
+Requires-Dist: mysql-connector-python
+Requires-Dist: bh_apistatus
+Requires-Dist: bh_utils
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: coverage; extra == "tests"
+Provides-Extra: builds
+Requires-Dist: build; extra == "builds"
+Requires-Dist: twine; extra == "builds"
+Provides-Extra: dev
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: myst-parser; extra == "dev"
+Requires-Dist: sphinx-rtd-theme; extra == "dev"
+
 # bh_database
 
 Database wrapper classes for SQLAlchemy.
 
 ## Pip installation
 
 ```
@@ -50,8 +80,8 @@
 
 ## Documentation
 
 [Full documentation](https://bh-database.readthedocs.io/)
 
 ## License
 
-[ MIT license ](http://www.opensource.org/licenses/mit-license.php)
+[ MIT license ](http://www.opensource.org/licenses/mit-license.php)
```

### Comparing `bh-database-0.0.4/pyproject.toml` & `bh_database-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bh-database"
-version = "0.0.4"
+version = "0.0.5"
 description = "Database wrapper classes for SQLAlchemy."
 
 readme = "README.md"
 authors = [{ name = "Van Be Hai Nguyen", email = "behai_nguyen@hotmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -33,15 +33,15 @@
   "pytest",
   "coverage"
 ]
 builds = [
     "build", 
     "twine"
 ]
-docs = [
+dev = [
     "sphinx",
     "myst-parser",
     "sphinx-rtd-theme"
 ]
 
 [project.urls]
 repository = "https://github.com/behai-nguyen/bh_database"
```

### Comparing `bh-database-0.0.4/src/bh_database/base_table.py` & `bh_database-0.0.5/src/bh_database/base_table.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.4/src/bh_database/constant.py` & `bh_database-0.0.5/src/bh_database/constant.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.4/src/bh_database/core.py` & `bh_database-0.0.5/src/bh_database/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,27 +50,28 @@
 
 from http import HTTPStatus
 
 from sqlalchemy import create_engine
 from sqlalchemy.orm import (
     sessionmaker, 
     scoped_session,
-    declarative_base,
+    DeclarativeBase,
     close_all_sessions,
     Query,
 )
 from sqlalchemy.orm.decl_api import DeclarativeMeta
 
 from bh_apistatus.result_status import ResultStatus
 
 from bh_database.paginator import Paginator
 
 #: 
-Base = declarative_base(metaclass=DeclarativeMeta)
-
+class Base(DeclarativeBase):
+    metaclass=DeclarativeMeta
+    
 class BaseQuery(Query):
     """Custom base query class.
 
     Provide pagination capability for `SQLAlchemy Query Object <https://docs.sqlalchemy.org/en/14/orm/query.html>`_.
 
     All models (tables) descend from :py:class:`BaseSQLAlchemy` will have their class attribute
     :attr:`~.BaseSQLAlchemy.query` set to this custom query class, therefore, automatically has 
@@ -122,32 +123,40 @@
     
 class BaseSQLAlchemy(Base, BaseModel):
     """The parent most class for all models / tables.
 
     Provide methods to implement transaction atomicity.
 
     Class attributes:
-        | session = None. When set, is of type `sqlalchemy.orm.session.Session <https://docs.sqlalchemy.org/en/20/orm/session_api.html#sqlalchemy.orm.Session>`_.
-        | query = None. When set, is of type :py:class:`BaseQuery`.
+        | session = None. When set, is of type `sqlalchemy.orm.session.Session <https://docs.sqlalchemy.org/en/20/orm/session_api.html#sqlalchemy.orm.Session>`_. This attribute is set after successfully calling the :py:class:`Database`'s :py:meth:`~.Database.connect` method.
+        |
+        | query = None. When set, is of type :py:class:`BaseQuery`. This attribute is set after successfully calling the :py:class:`Database`'s :py:meth:`~.Database.connect` method.
+
+    Application models, i.e. tables, descend indirectly from this class, and hence 
+    inherits attributes :attr:`~.session` and :attr:`~.query`. Table classes use 
+    these two class attributes to talk to the connected database: **they should 
+    not need the** :py:class:`Database` **class for anything else**.        
 
     In general, for this abstract class and its abstract descendant classes, do not 
     access :attr:`query` when not assigned. E.g.::
 
         assert core.BaseSQLAlchemy.query == None
 
     It results in the following exception::
 
         ArgumentError("Column expression, FROM clause, or other columns clause element expected, <class 'bh_database.core.BaseSQLAlchemy'>.")
     """
 
     __abstract__ = True
 
     #: Class attribute. When set, is of type `sqlalchemy.orm.session.Session <https://docs.sqlalchemy.org/en/20/orm/session_api.html#sqlalchemy.orm.Session>`_.
+    #: This attribute is set after successfully calling the :py:class:`Database`'s :py:meth:`~.Database.connect` method.
     session = None
     #: Class attribute. When set, is of type :py:class:`BaseQuery`.    
+    #: This attribute is set after successfully calling the :py:class:`Database`'s :py:meth:`~.Database.connect` method.
     query = None
 
     def begin_transaction(self):
         """Start a new transaction.
         """
         if not self.session.in_transaction(): self.session.begin()
```

### Comparing `bh-database-0.0.4/src/bh_database/paginator.py` & `bh_database-0.0.5/src/bh_database/paginator.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.4/src/bh_database.egg-info/PKG-INFO` & `bh_database-0.0.5/src/bh_database.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,36 @@
 Metadata-Version: 2.1
 Name: bh-database
-Version: 0.0.4
+Version: 0.0.5
 Summary: Database wrapper classes for SQLAlchemy.
 Author-email: Van Be Hai Nguyen <behai_nguyen@hotmail.com>
 Project-URL: repository, https://github.com/behai-nguyen/bh_database
 Project-URL: documentation, https://bh-database.readthedocs.io/
 Keywords: SQLAlchemy,database,wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: tomli; python_version >= "3.10"
+Requires-Dist: SQLAlchemy
+Requires-Dist: psycopg2-binary
+Requires-Dist: mysql-connector-python
+Requires-Dist: bh_apistatus
+Requires-Dist: bh_utils
 Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: coverage; extra == "tests"
 Provides-Extra: builds
-Provides-Extra: docs
+Requires-Dist: build; extra == "builds"
+Requires-Dist: twine; extra == "builds"
+Provides-Extra: dev
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: myst-parser; extra == "dev"
+Requires-Dist: sphinx-rtd-theme; extra == "dev"
 
 # bh_database
 
 Database wrapper classes for SQLAlchemy.
 
 ## Pip installation
```

### Comparing `bh-database-0.0.4/src/bh_database.egg-info/SOURCES.txt` & `bh_database-0.0.5/src/bh_database.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.4/tests/test_01_core_database_postgresql.py` & `bh_database-0.0.5/tests/test_01_core_database_postgresql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.4/tests/test_02_core_database_mysql.py` & `bh_database-0.0.5/tests/test_02_core_database_mysql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.4/tests/test_05_core_basesqlalchemy_postgresql.py` & `bh_database-0.0.5/tests/test_05_core_basesqlalchemy_postgresql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.4/tests/test_06_core_basesqlalchemy_mysql.py` & `bh_database-0.0.5/tests/test_06_core_basesqlalchemy_mysql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.4/tests/test_11_paginator_postgresql.py` & `bh_database-0.0.5/tests/test_11_paginator_postgresql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.4/tests/test_12_paginator_mysql.py` & `bh_database-0.0.5/tests/test_12_paginator_mysql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.4/tests/test_15_base_table_postgresql.py` & `bh_database-0.0.5/tests/test_15_base_table_postgresql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.4/tests/test_16_base_table_mysql.py` & `bh_database-0.0.5/tests/test_16_base_table_mysql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.4/tests/test_17_base_table_methods.py` & `bh_database-0.0.5/tests/test_17_base_table_methods.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.4/tests/test_20_base_table_dunder.py` & `bh_database-0.0.5/tests/test_20_base_table_dunder.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.4/tests/test_25_base_table_crud_methods_postgresql.py` & `bh_database-0.0.5/tests/test_25_base_table_crud_methods_postgresql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.4/tests/test_26_base_table_crud_methods_mysql.py` & `bh_database-0.0.5/tests/test_26_base_table_crud_methods_mysql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.4/tests/test_30_base_table_exception_postgresql.py` & `bh_database-0.0.5/tests/test_30_base_table_exception_postgresql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.4/tests/test_31_base_table_exception_mysql.py` & `bh_database-0.0.5/tests/test_31_base_table_exception_mysql.py`

 * *Files identical despite different names*

