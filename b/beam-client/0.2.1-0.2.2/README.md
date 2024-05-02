# Comparing `tmp/beam_client-0.2.1.tar.gz` & `tmp/beam_client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beam_client-0.2.1.tar", max compression
+gzip compressed data, was "beam_client-0.2.2.tar", max compression
```

## Comparing `beam_client-0.2.1.tar` & `beam_client-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1254 2024-04-02 19:22:26.042006 beam_client-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      637 2024-03-30 13:01:39.670148 beam_client-0.2.1/src/beam/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 02:07:20.445321 beam_client-0.2.1/src/beam/cli/__init__.py
--rw-r--r--   0        0        0      461 2024-03-29 14:37:29.406725 beam_client-0.2.1/src/beam/cli/logs.py
--rw-r--r--   0        0        0       83 2024-03-29 14:38:33.741973 beam_client-0.2.1/src/beam/cli/main.py
--rw-r--r--   0        0        0     1298 1970-01-01 00:00:00.000000 beam_client-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      736 2024-05-02 16:13:36.217308 beam_client-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      597 2024-04-17 13:15:05.679787 beam_client-0.2.2/src/beam/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:15:05.679851 beam_client-0.2.2/src/beam/cli/__init__.py
+-rw-r--r--   0        0        0      438 2024-04-29 21:55:36.161099 beam_client-0.2.2/src/beam/cli/logs.py
+-rw-r--r--   0        0        0      411 2024-05-02 13:57:53.572610 beam_client-0.2.2/src/beam/cli/main.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 beam_client-0.2.2/PKG-INFO
```

### Comparing `beam_client-0.2.1/src/beam/__init__.py` & `beam_client-0.2.2/src/beam/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 from beta9.abstractions.endpoint import Endpoint as endpoint
 from beta9.abstractions.function import Function as function
 from beta9.abstractions.image import Image
 from beta9.abstractions.map import Map
 from beta9.abstractions.queue import SimpleQueue as Queue
 from beta9.abstractions.taskqueue import TaskQueue as task_queue
 from beta9.abstractions.volume import Volume
-from beta9.type import type
 
 __version__ = "0.2.0"
 __all__ = [
     "__version__",
     "Map",
     "Image",
     "Queue",
     "Volume",
     "task_queue",
     "function",
     "endpoint",
     "Container",
-    "type",
 ]
```

