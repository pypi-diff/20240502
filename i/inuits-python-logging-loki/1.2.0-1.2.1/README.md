# Comparing `tmp/inuits_python_logging_loki-1.2.0.tar.gz` & `tmp/inuits_python_logging_loki-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inuits_python_logging_loki-1.2.0.tar", last modified: Tue Apr 30 14:49:50 2024, max compression
+gzip compressed data, was "inuits_python_logging_loki-1.2.1.tar", last modified: Thu May  2 07:42:08 2024, max compression
```

## Comparing `inuits_python_logging_loki-1.2.0.tar` & `inuits_python_logging_loki-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:49:50.853404 inuits_python_logging_loki-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-30 14:49:50.853404 inuits_python_logging_loki-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:49:50.853404 inuits_python_logging_loki-1.2.0/inuits_python_logging_loki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-30 14:49:50.000000 inuits_python_logging_loki-1.2.0/inuits_python_logging_loki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-30 14:49:50.000000 inuits_python_logging_loki-1.2.0/inuits_python_logging_loki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:49:50.000000 inuits_python_logging_loki-1.2.0/inuits_python_logging_loki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 14:49:50.000000 inuits_python_logging_loki-1.2.0/inuits_python_logging_loki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 14:49:50.000000 inuits_python_logging_loki-1.2.0/inuits_python_logging_loki.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:49:50.853404 inuits_python_logging_loki-1.2.0/logging_loki/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/logging_loki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/logging_loki/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/logging_loki/emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/logging_loki/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/logging_loki/json_loki_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/logging_loki/log_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/logging_loki/loki_context_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/logging_loki/loki_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 14:49:50.853404 inuits_python_logging_loki-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:49:50.853404 inuits_python_logging_loki-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-04-30 14:49:44.000000 inuits_python_logging_loki-1.2.0/tests/test_emitter_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:42:08.782215 inuits_python_logging_loki-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-02 07:41:59.000000 inuits_python_logging_loki-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-02 07:42:08.782215 inuits_python_logging_loki-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-02 07:41:59.000000 inuits_python_logging_loki-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:42:08.782215 inuits_python_logging_loki-1.2.1/inuits_python_logging_loki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-02 07:42:08.000000 inuits_python_logging_loki-1.2.1/inuits_python_logging_loki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-02 07:42:08.000000 inuits_python_logging_loki-1.2.1/inuits_python_logging_loki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 07:42:08.000000 inuits_python_logging_loki-1.2.1/inuits_python_logging_loki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 07:42:08.000000 inuits_python_logging_loki-1.2.1/inuits_python_logging_loki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 07:42:08.000000 inuits_python_logging_loki-1.2.1/inuits_python_logging_loki.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:42:08.782215 inuits_python_logging_loki-1.2.1/logging_loki/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-02 07:41:59.000000 inuits_python_logging_loki-1.2.1/logging_loki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-02 07:41:59.000000 inuits_python_logging_loki-1.2.1/logging_loki/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-05-02 07:41:59.000000 inuits_python_logging_loki-1.2.1/logging_loki/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-02 07:41:59.000000 inuits_python_logging_loki-1.2.1/logging_loki/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-02 07:41:59.000000 inuits_python_logging_loki-1.2.1/logging_loki/json_loki_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-02 07:41:59.000000 inuits_python_logging_loki-1.2.1/logging_loki/log_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-02 07:41:59.000000 inuits_python_logging_loki-1.2.1/logging_loki/loki_context_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-02 07:41:59.000000 inuits_python_logging_loki-1.2.1/logging_loki/loki_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-02 07:41:59.000000 inuits_python_logging_loki-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 07:42:08.782215 inuits_python_logging_loki-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:42:08.782215 inuits_python_logging_loki-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-02 07:41:59.000000 inuits_python_logging_loki-1.2.1/tests/test_emitter_v1.py
```

### Comparing `inuits_python_logging_loki-1.2.0/LICENSE` & `inuits_python_logging_loki-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.2.0/PKG-INFO` & `inuits_python_logging_loki-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inuits-python-logging-loki
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python logging handler for Grafana Loki.
 Author-email: Inuits <developers@inuits.eu>, Andrey Maslov <greyzmeem@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Andrey Maslov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `inuits_python_logging_loki-1.2.0/README.md` & `inuits_python_logging_loki-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.2.0/inuits_python_logging_loki.egg-info/PKG-INFO` & `inuits_python_logging_loki-1.2.1/inuits_python_logging_loki.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inuits-python-logging-loki
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python logging handler for Grafana Loki.
 Author-email: Inuits <developers@inuits.eu>, Andrey Maslov <greyzmeem@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Andrey Maslov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `inuits_python_logging_loki-1.2.0/inuits_python_logging_loki.egg-info/SOURCES.txt` & `inuits_python_logging_loki-1.2.1/inuits_python_logging_loki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.2.0/logging_loki/const.py` & `inuits_python_logging_loki-1.2.1/logging_loki/const.py`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.2.0/logging_loki/emitter.py` & `inuits_python_logging_loki-1.2.1/logging_loki/emitter.py`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.2.0/logging_loki/handlers.py` & `inuits_python_logging_loki-1.2.1/logging_loki/handlers.py`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.2.0/logging_loki/json_loki_logger.py` & `inuits_python_logging_loki-1.2.1/logging_loki/json_loki_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 
-from logging_loki import LokiLogger
+from .loki_logger import LokiLogger
 
 
 class JsonLokiLogger:
     def __init__(
             self, loki_logger: LokiLogger
     ):
         self._loki_logger = loki_logger
```

### Comparing `inuits_python_logging_loki-1.2.0/logging_loki/loki_context_logger.py` & `inuits_python_logging_loki-1.2.1/logging_loki/loki_context_logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import copy
-
-from logging_loki import LogContext
-from logging_loki import LokiLogger
+from .log_context import LogContext
+from .loki_logger import LokiLogger
 
 
 class LokiContextLogger:
     def __init__(self, logger: LokiLogger):
         self.logger = logger
         self.log_context = LogContext()
```

### Comparing `inuits_python_logging_loki-1.2.0/logging_loki/loki_logger.py` & `inuits_python_logging_loki-1.2.1/logging_loki/loki_logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import logging.handlers
 from multiprocessing import Queue
-from logging_loki import LokiHandler
+from .handlers import LokiHandler
 
 
 class LokiLogger:
     def __init__(
         self,
         loki_url: str | None = None,
         default_loki_labels: dict | None = None,
```

### Comparing `inuits_python_logging_loki-1.2.0/pyproject.toml` & `inuits_python_logging_loki-1.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=59.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inuits-python-logging-loki"
-version = "1.2.0"
+version = "1.2.1"
 description = "Python logging handler for Grafana Loki."
 readme = "README.md"
 authors = [{ name = "Inuits", email = "developers@inuits.eu" }, {name="Andrey Maslov", email="greyzmeem@gmail.com"}]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
```

### Comparing `inuits_python_logging_loki-1.2.0/tests/test_emitter_v1.py` & `inuits_python_logging_loki-1.2.1/tests/test_emitter_v1.py`

 * *Files identical despite different names*

