# Comparing `tmp/automizor-0.4.1.tar.gz` & `tmp/automizor-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automizor-0.4.1.tar", last modified: Thu May  2 12:17:02 2024, max compression
+gzip compressed data, was "automizor-0.4.2.tar", last modified: Thu May  2 15:56:24 2024, max compression
```

## Comparing `automizor-0.4.1.tar` & `automizor-0.4.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:17:02.728154 automizor-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-02 12:16:45.000000 automizor-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 12:16:45.000000 automizor-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 12:17:02.728154 automizor-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 12:16:45.000000 automizor-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:17:02.724154 automizor-0.4.1/automizor/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:17:02.724154 automizor-0.4.1/automizor/job/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/job/_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:17:02.724154 automizor-0.4.1/automizor/log/
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/log/_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:17:02.724154 automizor-0.4.1/automizor/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/storage/_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:17:02.724154 automizor-0.4.1/automizor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:17:02.728154 automizor-0.4.1/automizor/vault/
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/vault/_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/vault/_vault.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:17:02.728154 automizor-0.4.1/automizor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 12:17:02.000000 automizor-0.4.1/automizor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-02 12:17:02.000000 automizor-0.4.1/automizor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:17:02.000000 automizor-0.4.1/automizor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 12:17:02.000000 automizor-0.4.1/automizor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 12:17:02.000000 automizor-0.4.1/automizor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-02 12:17:02.728154 automizor-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-02 12:16:45.000000 automizor-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:24.075291 automizor-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-02 15:56:15.000000 automizor-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 15:56:15.000000 automizor-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 15:56:24.075291 automizor-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 15:56:15.000000 automizor-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:24.071291 automizor-0.4.2/automizor/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:24.071291 automizor-0.4.2/automizor/job/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/job/_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:24.071291 automizor-0.4.2/automizor/log/
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/log/_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:24.071291 automizor-0.4.2/automizor/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/storage/_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:24.071291 automizor-0.4.2/automizor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:24.071291 automizor-0.4.2/automizor/vault/
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/vault/_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-02 15:56:15.000000 automizor-0.4.2/automizor/vault/_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:24.075291 automizor-0.4.2/automizor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 15:56:24.000000 automizor-0.4.2/automizor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-02 15:56:24.000000 automizor-0.4.2/automizor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:56:24.000000 automizor-0.4.2/automizor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 15:56:24.000000 automizor-0.4.2/automizor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 15:56:24.000000 automizor-0.4.2/automizor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-02 15:56:24.075291 automizor-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-02 15:56:15.000000 automizor-0.4.2/setup.py
```

### Comparing `automizor-0.4.1/LICENSE` & `automizor-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `automizor-0.4.1/PKG-INFO` & `automizor-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automizor
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python Automizor framework
 Home-page: https://github.com/automizor/automizor-python
 Author: Christian Fischer
 Author-email: christian@automizor.io
 License: Apache License
 Keywords: automizor framework
 Classifier: Intended Audience :: Developers
```

### Comparing `automizor-0.4.1/automizor/exceptions.py` & `automizor-0.4.2/automizor/exceptions.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.1/automizor/job/__init__.py` & `automizor-0.4.2/automizor/job/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.1/automizor/job/_job.py` & `automizor-0.4.2/automizor/job/_job.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.1/automizor/log/__init__.py` & `automizor-0.4.2/automizor/log/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.1/automizor/log/_log.py` & `automizor-0.4.2/automizor/log/_log.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+from datetime import datetime, timezone
 from typing import Dict, List, Union
 
 LOG_LEVELS = {
     "DEBUG": 1,
     "INFO": 2,
     "WARNING": 3,
     "ERROR": 4,
@@ -81,11 +82,12 @@
         try:
             if os.path.exists(file_path):
                 with open(file_path, "r", encoding="utf-8") as file:
                     data = json.load(file)
         except json.JSONDecodeError:
             pass
 
-        data.append({"level": level, "msg": msg})
+        timestamp = datetime.now(timezone.utc).isoformat()
+        data.append({"level": level, "msg": msg, "timestamp": timestamp})
 
         with open(file_path, "w", encoding="utf-8") as file:
             json.dump(data, file, ensure_ascii=False)
```

### Comparing `automizor-0.4.1/automizor/storage/__init__.py` & `automizor-0.4.2/automizor/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.1/automizor/storage/_storage.py` & `automizor-0.4.2/automizor/storage/_storage.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.1/automizor/utils/__init__.py` & `automizor-0.4.2/automizor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.1/automizor/vault/__init__.py` & `automizor-0.4.2/automizor/vault/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.1/automizor/vault/_container.py` & `automizor-0.4.2/automizor/vault/_container.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.1/automizor/vault/_vault.py` & `automizor-0.4.2/automizor/vault/_vault.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.1/automizor.egg-info/PKG-INFO` & `automizor-0.4.2/automizor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automizor
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python Automizor framework
 Home-page: https://github.com/automizor/automizor-python
 Author: Christian Fischer
 Author-email: christian@automizor.io
 License: Apache License
 Keywords: automizor framework
 Classifier: Intended Audience :: Developers
```

### Comparing `automizor-0.4.1/automizor.egg-info/SOURCES.txt` & `automizor-0.4.2/automizor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automizor-0.4.1/setup.py` & `automizor-0.4.2/setup.py`

 * *Files identical despite different names*

