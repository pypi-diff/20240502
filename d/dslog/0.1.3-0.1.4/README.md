# Comparing `tmp/dslog-0.1.3.tar.gz` & `tmp/dslog-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dslog-0.1.3.tar", last modified: Thu May  2 07:55:16 2024, max compression
+gzip compressed data, was "dslog-0.1.4.tar", last modified: Thu May  2 07:56:49 2024, max compression
```

## Comparing `dslog-0.1.3.tar` & `dslog-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 07:55:16.109098 dslog-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      378 2024-05-02 07:55:16.109098 dslog-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      514 2024-05-02 07:55:13.000000 dslog-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-02 07:55:16.109098 dslog-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 07:55:16.099098 dslog-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 07:55:16.099098 dslog-0.1.3/src/dslog/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      468 2024-05-02 07:46:22.000000 dslog-0.1.3/src/dslog/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 07:55:16.099098 dslog-0.1.3/src/dslog/formatters/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-02 07:46:22.000000 dslog-0.1.3/src/dslog/formatters/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      108 2024-05-02 07:46:22.000000 dslog-0.1.3/src/dslog/formatters/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      437 2024-05-02 07:46:22.000000 dslog-0.1.3/src/dslog/formatters/formatters.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2081 2024-05-02 07:51:07.000000 dslog-0.1.3/src/dslog/logger.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 07:55:16.099098 dslog-0.1.3/src/dslog/loggers/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-02 07:46:22.000000 dslog-0.1.3/src/dslog/loggers/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-05-02 07:46:22.000000 dslog-0.1.3/src/dslog/loggers/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      502 2024-05-02 07:46:22.000000 dslog-0.1.3/src/dslog/loggers/_file.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       99 2024-05-02 07:46:22.000000 dslog-0.1.3/src/dslog/loggers/_rich.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      543 2024-05-02 07:46:22.000000 dslog-0.1.3/src/dslog/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 07:55:16.109098 dslog-0.1.3/src/dslog/util/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-02 07:46:22.000000 dslog-0.1.3/src/dslog/util/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1018 2024-05-02 07:46:22.000000 dslog-0.1.3/src/dslog/util/uvicorn.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 07:55:16.109098 dslog-0.1.3/src/dslog.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      378 2024-05-02 07:55:16.000000 dslog-0.1.3/src/dslog.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      509 2024-05-02 07:55:16.000000 dslog-0.1.3/src/dslog.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-02 07:55:16.000000 dslog-0.1.3/src/dslog.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-05-02 07:55:16.000000 dslog-0.1.3/src/dslog.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        6 2024-05-02 07:55:16.000000 dslog-0.1.3/src/dslog.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 07:56:49.499096 dslog-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1096 2024-05-02 07:56:49.499096 dslog-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      716 2024-05-02 07:56:47.000000 dslog-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      514 2024-05-02 07:56:47.000000 dslog-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-02 07:56:49.499096 dslog-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 07:56:49.499096 dslog-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 07:56:49.499096 dslog-0.1.4/src/dslog/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      468 2024-05-02 07:46:22.000000 dslog-0.1.4/src/dslog/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 07:56:49.499096 dslog-0.1.4/src/dslog/formatters/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-02 07:46:22.000000 dslog-0.1.4/src/dslog/formatters/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      108 2024-05-02 07:46:22.000000 dslog-0.1.4/src/dslog/formatters/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      437 2024-05-02 07:46:22.000000 dslog-0.1.4/src/dslog/formatters/formatters.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2081 2024-05-02 07:51:07.000000 dslog-0.1.4/src/dslog/logger.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 07:56:49.499096 dslog-0.1.4/src/dslog/loggers/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-02 07:46:22.000000 dslog-0.1.4/src/dslog/loggers/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-05-02 07:46:22.000000 dslog-0.1.4/src/dslog/loggers/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      502 2024-05-02 07:46:22.000000 dslog-0.1.4/src/dslog/loggers/_file.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       99 2024-05-02 07:46:22.000000 dslog-0.1.4/src/dslog/loggers/_rich.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      543 2024-05-02 07:46:22.000000 dslog-0.1.4/src/dslog/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 07:56:49.499096 dslog-0.1.4/src/dslog/util/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-02 07:46:22.000000 dslog-0.1.4/src/dslog/util/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1018 2024-05-02 07:46:22.000000 dslog-0.1.4/src/dslog/util/uvicorn.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 07:56:49.499096 dslog-0.1.4/src/dslog.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1096 2024-05-02 07:56:49.000000 dslog-0.1.4/src/dslog.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      519 2024-05-02 07:56:49.000000 dslog-0.1.4/src/dslog.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-02 07:56:49.000000 dslog-0.1.4/src/dslog.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-05-02 07:56:49.000000 dslog-0.1.4/src/dslog.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        6 2024-05-02 07:56:49.000000 dslog-0.1.4/src/dslog.egg-info/top_level.txt
```

### Comparing `dslog-0.1.3/pyproject.toml` & `dslog-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dslog"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Dead-simple logging: what python's logging should've been"
 dependencies = [
   "lazy-loader"
 ]
```

### Comparing `dslog-0.1.3/src/dslog/logger.py` & `dslog-0.1.4/src/dslog/logger.py`

 * *Files identical despite different names*

### Comparing `dslog-0.1.3/src/dslog/types.py` & `dslog-0.1.4/src/dslog/types.py`

 * *Files identical despite different names*

### Comparing `dslog-0.1.3/src/dslog/util/uvicorn.py` & `dslog-0.1.4/src/dslog/util/uvicorn.py`

 * *Files identical despite different names*

