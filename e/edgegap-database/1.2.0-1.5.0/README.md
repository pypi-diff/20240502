# Comparing `tmp/edgegap_database-1.2.0.tar.gz` & `tmp/edgegap_database-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_database-1.2.0.tar", max compression
+gzip compressed data, was "edgegap_database-1.5.0.tar", max compression
```

## Comparing `edgegap_database-1.2.0.tar` & `edgegap_database-1.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1993 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/LICENSE
--rw-r--r--   0        0        0     2180 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/README.md
--rw-r--r--   0        0        0       17 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/BUILD
--rw-r--r--   0        0        0      387 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/__init__.py
--rw-r--r--   0        0        0      625 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/_base.py
--rw-r--r--   0        0        0      452 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/_configuration.py
--rw-r--r--   0        0        0     1005 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/_engine.py
--rw-r--r--   0        0        0      885 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/_factory.py
--rw-r--r--   0        0        0      253 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/_model.py
--rw-r--r--   0        0        0     2555 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/_operator.py
--rw-r--r--   0        0        0      509 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/_session.py
--rw-r--r--   0        0        0       17 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/errors/BUILD
--rw-r--r--   0        0        0      327 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/errors/__init__.py
--rw-r--r--   0        0        0      698 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/errors/_exceptions.py
--rw-r--r--   0        0        0      484 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/errors/_factory.py
--rw-r--r--   0        0        0      743 2024-05-01 17:52:42.971603 edgegap_database-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2899 1970-01-01 00:00:00.000000 edgegap_database-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2180 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/README.md
+-rw-r--r--   0        0        0       17 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/BUILD
+-rw-r--r--   0        0        0      445 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/__init__.py
+-rw-r--r--   0        0        0      754 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/_base.py
+-rw-r--r--   0        0        0      580 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/_configuration.py
+-rw-r--r--   0        0        0     1072 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/_engine.py
+-rw-r--r--   0        0        0      796 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/_factory.py
+-rw-r--r--   0        0        0      271 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/_model.py
+-rw-r--r--   0        0        0     2339 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/_operator.py
+-rw-r--r--   0        0        0      509 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/_session.py
+-rw-r--r--   0        0        0       17 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/errors/BUILD
+-rw-r--r--   0        0        0      327 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/errors/__init__.py
+-rw-r--r--   0        0        0      698 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/errors/_exceptions.py
+-rw-r--r--   0        0        0      484 2024-05-02 18:20:19.987672 edgegap_database-1.5.0/edgegap_database/errors/_factory.py
+-rw-r--r--   0        0        0      743 2024-05-02 18:20:40.544195 edgegap_database-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2899 1970-01-01 00:00:00.000000 edgegap_database-1.5.0/PKG-INFO
```

### Comparing `edgegap_database-1.2.0/LICENSE` & `edgegap_database-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.2.0/README.md` & `edgegap_database-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.2.0/edgegap_database/_base.py` & `edgegap_database-1.5.0/edgegap_database/_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 class BaseModel(SQLModel, table=False):
     id: int | None = Field(default=None, primary_key=True)
     created_at: datetime | None = Field(
         default=None,
         sa_type=sa.DateTime(timezone=True),
         sa_column_kwargs={'server_default': sa.func.now()},
         nullable=False,
+        description='Timestamp when the object was created.',
     )
     updated_at: datetime | None = Field(
         default=None,
         sa_type=sa.DateTime(timezone=True),
         sa_column_kwargs={
             'onupdate': sa.func.now(),
             'server_default': sa.func.now(),
         },
+        description='Timestamp when the object was last updated.',
     )
```

### Comparing `edgegap_database-1.2.0/edgegap_database/_engine.py` & `edgegap_database-1.5.0/edgegap_database/_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
     class __Engine:
         def __init__(self, configuration: DatabaseConfiguration):
             self.__configuration = configuration
             self.__engine = create_engine(
                 url=str(self.__configuration.uri),
                 connect_args=self.__configuration.args or {},
+                poolclass=self.__configuration.pool_class or None,
             )
 
         def get_engine(self):
             return self.__engine
 
     def __init__(self, configuration: DatabaseConfiguration):
         key = configuration.application
```

### Comparing `edgegap_database-1.2.0/edgegap_database/_factory.py` & `edgegap_database-1.5.0/edgegap_database/_factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,24 +8,20 @@
 
 logger = logging.getLogger(__name__)
 
 
 class DatabaseConfigurationFactory:
     @staticmethod
     def __parse(conf: DatabaseConfiguration) -> DatabaseConfiguration:
-        if conf.application is None:
-            conf.application = 'DefaultApplicationName'
-
-        if not isinstance(conf.args, dict):
-            conf.args = {}
-
-        conf.args.update({
-            'application_name': conf.application,
-            'options': '-c timezone=utc',
-        })
+        if conf.uri.startswith('postgresql'):
+            conf.args.update({
+                'application_name': conf.application,
+                'options': '-c timezone=utc',
+            })
 
         return conf
 
-    def from_uri(self, uri: str | MultiHostUrl | PostgresDsn | SQLiteDsn, name: str) -> DatabaseConfiguration:
+    @classmethod
+    def from_uri(cls, uri: str | MultiHostUrl | PostgresDsn | SQLiteDsn, name: str) -> DatabaseConfiguration:
         configuration = DatabaseConfiguration(uri=str(uri), application=name)
 
-        return self.__parse(configuration)
+        return cls.__parse(configuration)
```

### Comparing `edgegap_database-1.2.0/edgegap_database/_operator.py` & `edgegap_database-1.5.0/edgegap_database/_operator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from datetime import datetime, timezone
+from contextlib import contextmanager
 from typing import Any
 
 from sqlalchemy.engine import ScalarResult, TupleResult
 from sqlmodel import Session, SQLModel
 from sqlmodel.sql import expression
 
 from .errors import DatabaseExceptionFactory
@@ -11,75 +11,69 @@
 logger = logging.getLogger(__name__)
 
 
 class DatabaseOperator:
     def __init__(self, session: Session):
         self.__session = session
 
+    @contextmanager
+    def handle_exception(self):
+        try:
+            yield
+        except Exception as e:
+            DatabaseExceptionFactory.handle(e)
+
     def all(self, statement: expression.Select | expression.SelectOfScalar) -> Any:
         return self.__session.exec(statement).all()
 
     def first(self, statement: expression.Select | expression.SelectOfScalar) -> Any:
         return self.__session.exec(statement).first()
 
     def exec(self, statement: expression.Select | expression.SelectOfScalar) -> TupleResult | ScalarResult:
         result = self.__session.exec(statement)
         self.__session.commit()
 
         return result
 
     def create(self, model: type(SQLModel)) -> type(SQLModel):
-        try:
+        with self.handle_exception():
             self.__session.add(model)
             self.__session.commit()
             self.__session.refresh(model)
 
             return model
-        except Exception as e:
-            DatabaseExceptionFactory.handle(e)
 
     def update(self, model: type(SQLModel)) -> type(SQLModel):
-        try:
-            if hasattr(model, 'updated_at'):
-                model.updated_at = datetime.now(tz=timezone.utc)
-
+        with self.handle_exception():
             self.__session.add(model)
             self.__session.commit()
             self.__session.refresh(model)
 
             return model
-        except Exception as e:
-            DatabaseExceptionFactory.handle(e)
 
     def update_many(self, models: list[type(SQLModel)]) -> list[type(SQLModel)]:
-        try:
+        with self.handle_exception():
             for model in models:
                 self.__session.add(model)
 
             self.__session.commit()
 
             for model in models:
                 self.__session.refresh(model)
 
             return models
-        except Exception as e:
-            DatabaseExceptionFactory.handle(e)
 
     def delete(self, model: type(SQLModel)) -> type(SQLModel):
-        try:
+        with self.handle_exception():
             self.__session.delete(model)
             self.__session.commit()
 
             return model
-        except Exception as e:
-            DatabaseExceptionFactory.handle(e)
 
     def delete_many(self, models: list[type(SQLModel)]) -> list[type(SQLModel)]:
-        try:
+        with self.handle_exception():
             for model in models:
                 self.__session.delete(model)
 
             self.__session.commit()
 
             return models
-        except Exception as e:
-            DatabaseExceptionFactory.handle(e)
```

### Comparing `edgegap_database-1.2.0/edgegap_database/errors/_exceptions.py` & `edgegap_database-1.5.0/edgegap_database/errors/_exceptions.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.2.0/pyproject.toml` & `edgegap_database-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-database"
-version = "1.2.0"
+version = "1.5.0"
 description = "The Edgegap Database library includes various tools and helpers for interacting with Database and Migrations. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 psycopg-c = "^3.1.18"
```

### Comparing `edgegap_database-1.2.0/PKG-INFO` & `edgegap_database-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-database
-Version: 1.2.0
+Version: 1.5.0
 Summary: The Edgegap Database library includes various tools and helpers for interacting with Database and Migrations. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

