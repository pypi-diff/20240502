# Comparing `tmp/peewee_async-0.9.0.tar.gz` & `tmp/peewee_async-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_async-0.9.0.tar", max compression
+gzip compressed data, was "peewee_async-0.9.1.tar", max compression
```

## Comparing `peewee_async-0.9.0.tar` & `peewee_async-0.9.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1096 2021-03-18 05:04:12.168926 peewee_async-0.9.0/LICENSE
--rw-r--r--   0        0        0     3020 2023-09-12 12:28:49.309769 peewee_async-0.9.0/README.md
--rw-r--r--   0        0        0    41031 2023-09-12 12:28:49.309769 peewee_async-0.9.0/peewee_async.py
--rw-r--r--   0        0        0      906 2023-09-13 04:54:32.068687 peewee_async-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     4132 1970-01-01 00:00:00.000000 peewee_async-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2021-03-18 05:04:12.168926 peewee_async-0.9.1/LICENSE
+-rw-r--r--   0        0        0     3020 2023-09-12 12:28:49.309769 peewee_async-0.9.1/README.md
+-rw-r--r--   0        0        0    41031 2023-09-12 12:28:49.309769 peewee_async-0.9.1/peewee_async.py
+-rw-r--r--   0        0        0     2927 2021-10-12 09:39:01.744442 peewee_async-0.9.1/peewee_asyncext.py
+-rw-r--r--   0        0        0      946 2023-09-14 05:32:12.218255 peewee_async-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4111 1970-01-01 00:00:00.000000 peewee_async-0.9.1/PKG-INFO
```

### Comparing `peewee_async-0.9.0/LICENSE` & `peewee_async-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `peewee_async-0.9.0/README.md` & `peewee_async-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `peewee_async-0.9.0/peewee_async.py` & `peewee_async-0.9.1/peewee_async.py`

 * *Files identical despite different names*

### Comparing `peewee_async-0.9.0/pyproject.toml` & `peewee_async-0.9.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 [tool.poetry]
 name = "peewee-async"
-version = "0.9.0"
+version = "0.9.1"
 description = "Asynchronous interface for peewee ORM powered by asyncio."
 authors = ["Alexey Kinev <rudy@05bit.com>", "Gorshkov Nikolay(contributor) <nogamemorebrain@gmail.com>"]
 readme = "README.md"
+packages = [
+    { include = "peewee_async.py" },
+    { include = "peewee_asyncext.py" },
+]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 peewee = "^3.15.4"
+importlib-metadata = "^6.7.0"
 
 aiopg = { version = "^1.4.0", optional = true }
 aiomysql = { version = "^0.2.0", optional = true }
 cryptography = { version = "^41.0.3", optional = true }
 pytest = { version = "^7.4.1", optional = true }
 pytest-asyncio = { version = "^0.21.1", optional = true }
-importlib-metadata= { version = "^6.7.0", optional = true }
 
 
 [tool.poetry.extras]
 postgresql = ["aiopg"]
 mysql = ["aiomysql", "cryptography"]
-develop = ["aiopg", "aiomysql", "cryptography", "importlib-metadata", "pytest", "pytest-asyncio"]
+develop = ["aiopg", "aiomysql", "cryptography", "pytest", "pytest-asyncio"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `peewee_async-0.9.0/PKG-INFO` & `peewee_async-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-async
-Version: 0.9.0
+Version: 0.9.1
 Summary: Asynchronous interface for peewee ORM powered by asyncio.
 Author: Alexey Kinev
 Author-email: rudy@05bit.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: develop
 Provides-Extra: mysql
 Provides-Extra: postgresql
 Requires-Dist: aiomysql (>=0.2.0,<0.3.0) ; extra == "mysql" or extra == "develop"
 Requires-Dist: aiopg (>=1.4.0,<2.0.0) ; extra == "postgresql" or extra == "develop"
 Requires-Dist: cryptography (>=41.0.3,<42.0.0) ; extra == "mysql" or extra == "develop"
-Requires-Dist: importlib-metadata (>=6.7.0,<7.0.0) ; extra == "develop"
+Requires-Dist: importlib-metadata (>=6.7.0,<7.0.0)
 Requires-Dist: peewee (>=3.15.4,<4.0.0)
 Requires-Dist: pytest (>=7.4.1,<8.0.0) ; extra == "develop"
 Requires-Dist: pytest-asyncio (>=0.21.1,<0.22.0) ; extra == "develop"
 Description-Content-Type: text/markdown
 
 peewee-async
 ============
```

