# Comparing `tmp/automizor-0.4.2.tar.gz` & `tmp/automizor-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automizor-0.4.2.tar", last modified: Thu May  2 15:56:24 2024, max compression
+gzip compressed data, was "automizor-0.4.3.tar", last modified: Thu May  2 16:30:47 2024, max compression
```

## Comparing `automizor-0.4.2.tar` & `automizor-0.4.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:24.075291 automizor-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-02 15:56:15.000000 automizor-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 15:56:15.000000 automizor-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 15:56:24.075291 automizor-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 15:56:15.000000 automizor-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:24.071291 automizor-0.4.2/automizor/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:24.071291 automizor-0.4.2/automizor/job/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/job/_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:24.071291 automizor-0.4.2/automizor/log/
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/log/_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:24.071291 automizor-0.4.2/automizor/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/storage/_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:24.071291 automizor-0.4.2/automizor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:24.071291 automizor-0.4.2/automizor/vault/
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/vault/_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/vault/_vault.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:24.075291 automizor-0.4.2/automizor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 15:56:24.000000 automizor-0.4.2/automizor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-02 15:56:24.000000 automizor-0.4.2/automizor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:56:24.000000 automizor-0.4.2/automizor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 15:56:24.000000 automizor-0.4.2/automizor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 15:56:24.000000 automizor-0.4.2/automizor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-02 15:56:24.075291 automizor-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-02 15:56:15.000000 automizor-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:30:47.915626 automizor-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-02 16:30:39.000000 automizor-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 16:30:39.000000 automizor-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 16:30:47.915626 automizor-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 16:30:39.000000 automizor-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:30:47.911626 automizor-0.4.3/automizor/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 16:30:39.000000 automizor-0.4.3/automizor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-02 16:30:39.000000 automizor-0.4.3/automizor/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:30:47.915626 automizor-0.4.3/automizor/job/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-02 16:30:39.000000 automizor-0.4.3/automizor/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-02 16:30:39.000000 automizor-0.4.3/automizor/job/_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:30:47.915626 automizor-0.4.3/automizor/log/
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-02 16:30:39.000000 automizor-0.4.3/automizor/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-02 16:30:39.000000 automizor-0.4.3/automizor/log/_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:30:47.915626 automizor-0.4.3/automizor/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-02 16:30:39.000000 automizor-0.4.3/automizor/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-05-02 16:30:39.000000 automizor-0.4.3/automizor/storage/_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:30:47.915626 automizor-0.4.3/automizor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-02 16:30:39.000000 automizor-0.4.3/automizor/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:30:47.915626 automizor-0.4.3/automizor/vault/
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-02 16:30:39.000000 automizor-0.4.3/automizor/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-02 16:30:39.000000 automizor-0.4.3/automizor/vault/_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-02 16:30:39.000000 automizor-0.4.3/automizor/vault/_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:30:47.915626 automizor-0.4.3/automizor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 16:30:47.000000 automizor-0.4.3/automizor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-02 16:30:47.000000 automizor-0.4.3/automizor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:30:47.000000 automizor-0.4.3/automizor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 16:30:47.000000 automizor-0.4.3/automizor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 16:30:47.000000 automizor-0.4.3/automizor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-02 16:30:47.915626 automizor-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-02 16:30:39.000000 automizor-0.4.3/setup.py
```

### Comparing `automizor-0.4.2/LICENSE` & `automizor-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `automizor-0.4.2/PKG-INFO` & `automizor-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automizor
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python Automizor framework
 Home-page: https://github.com/automizor/automizor-python
 Author: Christian Fischer
 Author-email: christian@automizor.io
 License: Apache License
 Keywords: automizor framework
 Classifier: Intended Audience :: Developers
```

### Comparing `automizor-0.4.2/automizor/exceptions.py` & `automizor-0.4.3/automizor/exceptions.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.2/automizor/job/__init__.py` & `automizor-0.4.3/automizor/job/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.2/automizor/job/_job.py` & `automizor-0.4.3/automizor/job/_job.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.2/automizor/log/__init__.py` & `automizor-0.4.3/automizor/log/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 from functools import lru_cache
 
-from ._log import JSON
+from ._log import VALUE
 
 
 @lru_cache
 def _get_log():
     from ._log import Log
 
     return Log()
 
 
-def debug(msg: JSON):
+def debug(msg: VALUE):
     """
     Writes a debug log message with a level of "DEBUG".
 
     Parameters:
-        msg (JSON): The log message to write. This can be a string, number, boolean, dictionary,
-            list, or None.
+        msg (VALUE): The log message to write. This can be a boolean, string, bytes, integer,
+            or float value.
     """
 
     _get_log().write_log("DEBUG", msg)
 
 
-def info(msg: JSON):
+def info(msg: VALUE):
     """
     Writes an info log message with a level of "INFO".
 
     Parameters:
-        msg (JSON): The log message to write. This can be a string, number, boolean, dictionary,
-            list, or None.
+        msg (VALUE): The log message to write. This can be a boolean, string, bytes, integer,
+            or float value.
     """
 
     _get_log().write_log("INFO", msg)
 
 
-def warning(msg: JSON):
+def warning(msg: VALUE):
     """
     Writes a warning log message with a level of "WARNING".
 
     Parameters:
-        msg (JSON): The log message to write. This can be a string, number, boolean, dictionary,
-            list, or None.
+        msg (VALUE): The log message to write. This can be a boolean, string, bytes, integer,
+            or float value.
     """
 
     _get_log().write_log("WARNING", msg)
 
 
-def error(msg: JSON):
+def error(msg: VALUE):
     """
     Writes an error log message with a level of "ERROR".
 
     Parameters:
-        msg (JSON): The log message to write. This can be a string, number, boolean, dictionary,
-            list, or None.
+        msg (VALUE): The log message to write. This can be a boolean, string, bytes, integer,
+            or float value.
     """
 
     _get_log().write_log("ERROR", msg)
 
 
-def critical(msg: JSON):
+def critical(msg: VALUE):
     """
     Writes a critical log message with a level of "CRITICAL".
 
     Parameters:
-        msg (JSON): The log message to write. This can be a string, number, boolean, dictionary,
-            list, or None.
+        msg (VALUE): The log message to write. This can be a boolean, string, bytes, integer,
+            or float value.
     """
 
     _get_log().write_log("CRITICAL", msg)
 
 
 def set_level(level: str):
     """
```

### Comparing `automizor-0.4.2/automizor/log/_log.py` & `automizor-0.4.3/automizor/log/_log.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import json
 import os
 from datetime import datetime, timezone
-from typing import Dict, List, Union
+from typing import Union
 
 LOG_LEVELS = {
     "DEBUG": 1,
     "INFO": 2,
     "WARNING": 3,
     "ERROR": 4,
     "CRITICAL": 5,
 }
 
-JSON = Union[str, int, float, bool, None, Dict[str, "JSON"], List["JSON"]]
+VALUE = Union[bool, str, bytes, int, float]
 
 
 class Log:
     """
     `Log` is a class that facilitates logging messages to a local file, which can be
     useful for debugging and monitoring purposes. It provides a simple interface for
     writing log messages with different levels, such as "info", "warning", "error", etc.
@@ -30,15 +30,15 @@
 
         from automizor import log
 
         # Set log level to INFO
         log.set_level("INFO")
 
         # Write a log message
-        log.info({"key": "value"})
+        log.info("This is an info message")
     """
 
     def __init__(self):
         self.level = "INFO"
 
     def set_level(self, level: str):
         """
@@ -53,23 +53,23 @@
         """
 
         if level not in LOG_LEVELS:
             raise ValueError(f"Invalid log level: {level}")
 
         self.level = level
 
-    def write_log(self, level: str, msg: JSON):
+    def write_log(self, level: str, msg: VALUE):
         """
         Write a log message with the specified log level.
 
         Parameters:
             level (str): The log level of the message. Valid log levels are "DEBUG", "INFO",
                 "WARNING", "ERROR", and "CRITICAL".
-            msg (JSON): The log message to write. This can be a string, number, boolean, dictionary,
-                list, or None.
+            msg (VALUE): The log message to write. This can be a boolean, string, bytes, integer,
+                or float value.
 
         Raises:
             ValueError: If an invalid log level is provided.
         """
 
         if level not in LOG_LEVELS:
             raise ValueError(f"Invalid log level: {level}")
```

### Comparing `automizor-0.4.2/automizor/storage/__init__.py` & `automizor-0.4.3/automizor/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.2/automizor/storage/_storage.py` & `automizor-0.4.3/automizor/storage/_storage.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.2/automizor/utils/__init__.py` & `automizor-0.4.3/automizor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.2/automizor/vault/__init__.py` & `automizor-0.4.3/automizor/vault/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.2/automizor/vault/_container.py` & `automizor-0.4.3/automizor/vault/_container.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.2/automizor/vault/_vault.py` & `automizor-0.4.3/automizor/vault/_vault.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.2/automizor.egg-info/PKG-INFO` & `automizor-0.4.3/automizor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automizor
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python Automizor framework
 Home-page: https://github.com/automizor/automizor-python
 Author: Christian Fischer
 Author-email: christian@automizor.io
 License: Apache License
 Keywords: automizor framework
 Classifier: Intended Audience :: Developers
```

### Comparing `automizor-0.4.2/automizor.egg-info/SOURCES.txt` & `automizor-0.4.3/automizor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automizor-0.4.2/setup.py` & `automizor-0.4.3/setup.py`

 * *Files identical despite different names*

