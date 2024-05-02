# Comparing `tmp/qai_server-0.5.0.tar.gz` & `tmp/qai_server-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qai_server-0.5.0.tar", max compression
+gzip compressed data, was "qai_server-0.5.1.tar", max compression
```

## Comparing `qai_server-0.5.0.tar` & `qai_server-0.5.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       17 2024-04-19 20:20:41.923099 qai_server-0.5.0/README.md
--rw-r--r--   0        0        0     1181 2024-05-02 06:06:27.689019 qai_server-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1168 2024-04-30 20:35:10.418212 qai_server-0.5.0/src/qai/server/__init__.py
--rw-r--r--   0        0        0      159 2024-04-19 22:02:46.638364 qai_server-0.5.0/src/qai/server/config.py
--rw-r--r--   0        0        0     2249 2024-04-29 04:11:00.509739 qai_server-0.5.0/src/qai/server/mock_responses.py
--rw-r--r--   0        0        0     3064 2024-05-01 03:39:19.096752 qai_server-0.5.0/src/qai/server/models.py
--rw-r--r--   0        0        0     5876 2024-05-01 03:45:06.872714 qai_server-0.5.0/src/qai/server/serve.py
--rw-r--r--   0        0        0        0 2024-04-19 21:43:15.360059 qai_server-0.5.0/src/qai/server/tools/__init__.py
--rw-r--r--   0        0        0     2870 2024-04-30 19:58:26.080497 qai_server-0.5.0/src/qai/server/tools/security.py
--rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 qai_server-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-04-19 20:20:41.923099 qai_server-0.5.1/README.md
+-rw-r--r--   0        0        0     1181 2024-05-02 06:07:56.422448 qai_server-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1168 2024-04-30 20:35:10.418212 qai_server-0.5.1/src/qai/server/__init__.py
+-rw-r--r--   0        0        0      159 2024-04-19 22:02:46.638364 qai_server-0.5.1/src/qai/server/config.py
+-rw-r--r--   0        0        0     2249 2024-04-29 04:11:00.509739 qai_server-0.5.1/src/qai/server/mock_responses.py
+-rw-r--r--   0        0        0     3064 2024-05-01 03:39:19.096752 qai_server-0.5.1/src/qai/server/models.py
+-rw-r--r--   0        0        0     5876 2024-05-01 03:45:06.872714 qai_server-0.5.1/src/qai/server/serve.py
+-rw-r--r--   0        0        0        0 2024-04-19 21:43:15.360059 qai_server-0.5.1/src/qai/server/tools/__init__.py
+-rw-r--r--   0        0        0     2870 2024-04-30 19:58:26.080497 qai_server-0.5.1/src/qai/server/tools/security.py
+-rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 qai_server-0.5.1/PKG-INFO
```

### Comparing `qai_server-0.5.0/pyproject.toml` & `qai_server-0.5.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.poetry]
 authors = ["parnell <152523161+leeparnell@users.noreply.github.com>"]
 description = ""
 name = "qai-server"
 packages = [{from = "src", include = "qai"}]
 readme = "README.md"
-version = "0.5.0"
+version = "0.5.1"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 beautifulsoup4 = "^4.12.2"
 dataclasses-json = "^0.6.4"
 flask = "^3.0.3"
 flask-pydantic = "^0.12.0"
```

### Comparing `qai_server-0.5.0/src/qai/server/__init__.py` & `qai_server-0.5.1/src/qai/server/__init__.py`

 * *Files identical despite different names*

### Comparing `qai_server-0.5.0/src/qai/server/mock_responses.py` & `qai_server-0.5.1/src/qai/server/mock_responses.py`

 * *Files identical despite different names*

### Comparing `qai_server-0.5.0/src/qai/server/models.py` & `qai_server-0.5.1/src/qai/server/models.py`

 * *Files identical despite different names*

### Comparing `qai_server-0.5.0/src/qai/server/serve.py` & `qai_server-0.5.1/src/qai/server/serve.py`

 * *Files identical despite different names*

### Comparing `qai_server-0.5.0/src/qai/server/tools/security.py` & `qai_server-0.5.1/src/qai/server/tools/security.py`

 * *Files identical despite different names*

### Comparing `qai_server-0.5.0/PKG-INFO` & `qai_server-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qai-server
-Version: 0.5.0
+Version: 0.5.1
 Summary: 
 Author: parnell
 Author-email: 152523161+leeparnell@users.noreply.github.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
```

