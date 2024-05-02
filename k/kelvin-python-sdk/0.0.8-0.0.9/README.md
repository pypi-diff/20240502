# Comparing `tmp/kelvin-python-sdk-0.0.8.tar.gz` & `tmp/kelvin-python-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kelvin-python-sdk-0.0.8.tar", last modified: Fri Oct 20 17:52:16 2023, max compression
+gzip compressed data, was "kelvin-python-sdk-0.0.9.tar", last modified: Thu Oct 26 16:59:37 2023, max compression
```

## Comparing `kelvin-python-sdk-0.0.8.tar` & `kelvin-python-sdk-0.0.9.tar`

### file list

```diff
@@ -1,51 +1,55 @@
-drwxr-xr-x   0 joaomota   (501) staff       (20)        0 2023-10-20 17:52:16.281027 kelvin-python-sdk-0.0.8/
--rw-r--r--   0 joaomota   (501) staff       (20)     1520 2023-08-30 22:30:59.000000 kelvin-python-sdk-0.0.8/.gitignore
--rw-r--r--   0 joaomota   (501) staff       (20)     3728 2023-09-13 18:30:11.000000 kelvin-python-sdk-0.0.8/Jenkinsfile
--rw-r--r--   0 joaomota   (501) staff       (20)     1766 2023-10-20 17:52:16.280589 kelvin-python-sdk-0.0.8/PKG-INFO
--rw-r--r--   0 joaomota   (501) staff       (20)      565 2023-08-30 22:30:59.000000 kelvin-python-sdk-0.0.8/README.md
--rw-r--r--   0 joaomota   (501) staff       (20)      460 2023-09-14 02:19:55.000000 kelvin-python-sdk-0.0.8/constraints.txt
-drwxr-xr-x   0 joaomota   (501) staff       (20)        0 2023-10-20 17:52:16.271475 kelvin-python-sdk-0.0.8/examples/
--rw-r--r--   0 joaomota   (501) staff       (20)     3628 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.8/examples/example.py
--rw-r--r--   0 joaomota   (501) staff       (20)     1724 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.8/examples/example.yaml
--rw-r--r--   0 joaomota   (501) staff       (20)     1554 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.8/examples/subscriber.py
-drwxr-xr-x   0 joaomota   (501) staff       (20)        0 2023-10-20 17:52:16.271929 kelvin-python-sdk-0.0.8/kelvin/
-drwxr-xr-x   0 joaomota   (501) staff       (20)        0 2023-10-20 17:52:16.273904 kelvin-python-sdk-0.0.8/kelvin/app/
--rw-r--r--   0 joaomota   (501) staff       (20)      195 2023-10-06 12:55:42.000000 kelvin-python-sdk-0.0.8/kelvin/app/__init__.py
--rw-r--r--   0 joaomota   (501) staff       (20)    11552 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.8/kelvin/app/client.py
--rw-r--r--   0 joaomota   (501) staff       (20)      833 2023-10-20 17:50:42.000000 kelvin-python-sdk-0.0.8/kelvin/app/config_msg.py
--rw-r--r--   0 joaomota   (501) staff       (20)     1118 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.8/kelvin/app/filters.py
--rw-r--r--   0 joaomota   (501) staff       (20)     4845 2023-10-20 17:50:42.000000 kelvin-python-sdk-0.0.8/kelvin/app/msg_builders.py
--rw-r--r--   0 joaomota   (501) staff       (20)     2527 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.8/kelvin/app/stream.py
--rw-r--r--   0 joaomota   (501) staff       (20)      645 2023-09-13 18:30:11.000000 kelvin-python-sdk-0.0.8/kelvin/logs.py
-drwxr-xr-x   0 joaomota   (501) staff       (20)        0 2023-10-20 17:52:16.275794 kelvin-python-sdk-0.0.8/kelvin/message/
--rw-r--r--   0 joaomota   (501) staff       (20)     1371 2023-10-06 12:55:42.000000 kelvin-python-sdk-0.0.8/kelvin/message/__init__.py
--rw-r--r--   0 joaomota   (501) staff       (20)     3215 2023-10-20 17:50:42.000000 kelvin-python-sdk-0.0.8/kelvin/message/base_messages.py
--rw-r--r--   0 joaomota   (501) staff       (20)     8618 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.8/kelvin/message/krn.py
--rw-r--r--   0 joaomota   (501) staff       (20)     6436 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.8/kelvin/message/message.py
--rw-r--r--   0 joaomota   (501) staff       (20)     4544 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.8/kelvin/message/msg_type.py
--rw-r--r--   0 joaomota   (501) staff       (20)      882 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.8/kelvin/message/primitives.py
--rw-r--r--   0 joaomota   (501) staff       (20)      910 2023-09-13 18:30:11.000000 kelvin-python-sdk-0.0.8/kelvin/message/utils.py
-drwxr-xr-x   0 joaomota   (501) staff       (20)        0 2023-10-20 17:52:16.276677 kelvin-python-sdk-0.0.8/kelvin/publisher/
--rw-r--r--   0 joaomota   (501) staff       (20)      105 2023-09-14 02:19:55.000000 kelvin-python-sdk-0.0.8/kelvin/publisher/__init__.py
--rw-r--r--   0 joaomota   (501) staff       (20)     1248 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.8/kelvin/publisher/config.py
--rw-r--r--   0 joaomota   (501) staff       (20)     2244 2023-10-20 17:50:42.000000 kelvin-python-sdk-0.0.8/kelvin/publisher/main.py
--rw-r--r--   0 joaomota   (501) staff       (20)     6161 2023-10-20 17:50:42.000000 kelvin-python-sdk-0.0.8/kelvin/publisher/publisher.py
-drwxr-xr-x   0 joaomota   (501) staff       (20)        0 2023-10-20 17:52:16.277528 kelvin-python-sdk-0.0.8/kelvin_python_sdk.egg-info/
--rw-r--r--   0 joaomota   (501) staff       (20)     1766 2023-10-20 17:52:16.000000 kelvin-python-sdk-0.0.8/kelvin_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 joaomota   (501) staff       (20)     1015 2023-10-20 17:52:16.000000 kelvin-python-sdk-0.0.8/kelvin_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 joaomota   (501) staff       (20)        1 2023-10-20 17:52:16.000000 kelvin-python-sdk-0.0.8/kelvin_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 joaomota   (501) staff       (20)       64 2023-10-20 17:52:16.000000 kelvin-python-sdk-0.0.8/kelvin_python_sdk.egg-info/entry_points.txt
--rw-r--r--   0 joaomota   (501) staff       (20)      263 2023-10-20 17:52:16.000000 kelvin-python-sdk-0.0.8/kelvin_python_sdk.egg-info/requires.txt
--rw-r--r--   0 joaomota   (501) staff       (20)        7 2023-10-20 17:52:16.000000 kelvin-python-sdk-0.0.8/kelvin_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 joaomota   (501) staff       (20)     1881 2023-10-06 12:55:42.000000 kelvin-python-sdk-0.0.8/pyproject.toml
--rw-r--r--   0 joaomota   (501) staff       (20)       36 2023-09-14 02:19:55.000000 kelvin-python-sdk-0.0.8/requirements.in
--rw-r--r--   0 joaomota   (501) staff       (20)      606 2023-09-14 02:19:55.000000 kelvin-python-sdk-0.0.8/requirements.txt
--rw-r--r--   0 joaomota   (501) staff       (20)       38 2023-10-20 17:52:16.281103 kelvin-python-sdk-0.0.8/setup.cfg
-drwxr-xr-x   0 joaomota   (501) staff       (20)        0 2023-10-20 17:52:16.279316 kelvin-python-sdk-0.0.8/tests/
--rw-r--r--   0 joaomota   (501) staff       (20)     2880 2023-10-20 17:50:42.000000 kelvin-python-sdk-0.0.8/tests/test_client.py
--rw-r--r--   0 joaomota   (501) staff       (20)     1859 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.8/tests/test_client_calbacks.py
--rw-r--r--   0 joaomota   (501) staff       (20)      348 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.8/tests/test_filters.py
--rw-r--r--   0 joaomota   (501) staff       (20)     9089 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.8/tests/test_message.py
--rw-r--r--   0 joaomota   (501) staff       (20)     1057 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.8/tests/test_message_builders.py
--rw-r--r--   0 joaomota   (501) staff       (20)      407 2023-09-13 18:30:11.000000 kelvin-python-sdk-0.0.8/tests/test_utils.py
--rw-r--r--   0 joaomota   (501) staff       (20)      652 2023-10-06 12:55:42.000000 kelvin-python-sdk-0.0.8/tox.ini
+drwxr-xr-x   0 joaomota   (501) staff       (20)        0 2023-10-26 16:59:37.215177 kelvin-python-sdk-0.0.9/
+-rw-r--r--   0 joaomota   (501) staff       (20)     1520 2023-08-30 22:30:59.000000 kelvin-python-sdk-0.0.9/.gitignore
+-rw-r--r--   0 joaomota   (501) staff       (20)     3728 2023-09-13 18:30:11.000000 kelvin-python-sdk-0.0.9/Jenkinsfile
+-rw-r--r--   0 joaomota   (501) staff       (20)     1859 2023-10-26 16:59:37.214791 kelvin-python-sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 joaomota   (501) staff       (20)      565 2023-08-30 22:30:59.000000 kelvin-python-sdk-0.0.9/README.md
+-rw-r--r--   0 joaomota   (501) staff       (20)      487 2023-10-26 16:54:14.000000 kelvin-python-sdk-0.0.9/constraints.txt
+drwxr-xr-x   0 joaomota   (501) staff       (20)        0 2023-10-26 16:59:37.204618 kelvin-python-sdk-0.0.9/examples/
+drwxr-xr-x   0 joaomota   (501) staff       (20)        0 2023-10-26 16:59:37.205523 kelvin-python-sdk-0.0.9/examples/csv/
+-rw-r--r--   0 joaomota   (501) staff       (20)      808 2023-10-26 16:54:14.000000 kelvin-python-sdk-0.0.9/examples/csv/csv_app.py
+-rw-r--r--   0 joaomota   (501) staff       (20)     1092 2023-10-26 16:54:14.000000 kelvin-python-sdk-0.0.9/examples/csv/csv_app.yaml
+-rw-r--r--   0 joaomota   (501) staff       (20)      671 2023-10-26 16:54:14.000000 kelvin-python-sdk-0.0.9/examples/csv/data.csv
+-rw-r--r--   0 joaomota   (501) staff       (20)     3628 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.9/examples/example.py
+-rw-r--r--   0 joaomota   (501) staff       (20)     1724 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.9/examples/example.yaml
+-rw-r--r--   0 joaomota   (501) staff       (20)     1554 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.9/examples/subscriber.py
+drwxr-xr-x   0 joaomota   (501) staff       (20)        0 2023-10-26 16:59:37.205697 kelvin-python-sdk-0.0.9/kelvin/
+drwxr-xr-x   0 joaomota   (501) staff       (20)        0 2023-10-26 16:59:37.207731 kelvin-python-sdk-0.0.9/kelvin/app/
+-rw-r--r--   0 joaomota   (501) staff       (20)      195 2023-10-06 12:55:42.000000 kelvin-python-sdk-0.0.9/kelvin/app/__init__.py
+-rw-r--r--   0 joaomota   (501) staff       (20)    12014 2023-10-26 16:54:14.000000 kelvin-python-sdk-0.0.9/kelvin/app/client.py
+-rw-r--r--   0 joaomota   (501) staff       (20)      833 2023-10-20 17:50:42.000000 kelvin-python-sdk-0.0.9/kelvin/app/config_msg.py
+-rw-r--r--   0 joaomota   (501) staff       (20)     1118 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.9/kelvin/app/filters.py
+-rw-r--r--   0 joaomota   (501) staff       (20)     4845 2023-10-20 17:50:42.000000 kelvin-python-sdk-0.0.9/kelvin/app/msg_builders.py
+-rw-r--r--   0 joaomota   (501) staff       (20)     2527 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.9/kelvin/app/stream.py
+-rw-r--r--   0 joaomota   (501) staff       (20)      645 2023-09-13 18:30:11.000000 kelvin-python-sdk-0.0.9/kelvin/logs.py
+drwxr-xr-x   0 joaomota   (501) staff       (20)        0 2023-10-26 16:59:37.209602 kelvin-python-sdk-0.0.9/kelvin/message/
+-rw-r--r--   0 joaomota   (501) staff       (20)     1371 2023-10-06 12:55:42.000000 kelvin-python-sdk-0.0.9/kelvin/message/__init__.py
+-rw-r--r--   0 joaomota   (501) staff       (20)     3215 2023-10-20 17:50:42.000000 kelvin-python-sdk-0.0.9/kelvin/message/base_messages.py
+-rw-r--r--   0 joaomota   (501) staff       (20)     8593 2023-10-26 16:54:14.000000 kelvin-python-sdk-0.0.9/kelvin/message/krn.py
+-rw-r--r--   0 joaomota   (501) staff       (20)     6408 2023-10-26 16:54:14.000000 kelvin-python-sdk-0.0.9/kelvin/message/message.py
+-rw-r--r--   0 joaomota   (501) staff       (20)     4504 2023-10-26 16:54:14.000000 kelvin-python-sdk-0.0.9/kelvin/message/msg_type.py
+-rw-r--r--   0 joaomota   (501) staff       (20)      882 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.9/kelvin/message/primitives.py
+-rw-r--r--   0 joaomota   (501) staff       (20)      910 2023-09-13 18:30:11.000000 kelvin-python-sdk-0.0.9/kelvin/message/utils.py
+drwxr-xr-x   0 joaomota   (501) staff       (20)        0 2023-10-26 16:59:37.210557 kelvin-python-sdk-0.0.9/kelvin/publisher/
+-rw-r--r--   0 joaomota   (501) staff       (20)        0 2023-10-26 16:54:14.000000 kelvin-python-sdk-0.0.9/kelvin/publisher/__init__.py
+-rw-r--r--   0 joaomota   (501) staff       (20)     1248 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.9/kelvin/publisher/config.py
+-rw-r--r--   0 joaomota   (501) staff       (20)     4340 2023-10-26 16:54:14.000000 kelvin-python-sdk-0.0.9/kelvin/publisher/main.py
+-rw-r--r--   0 joaomota   (501) staff       (20)    12860 2023-10-26 16:54:14.000000 kelvin-python-sdk-0.0.9/kelvin/publisher/publisher.py
+drwxr-xr-x   0 joaomota   (501) staff       (20)        0 2023-10-26 16:59:37.211537 kelvin-python-sdk-0.0.9/kelvin_python_sdk.egg-info/
+-rw-r--r--   0 joaomota   (501) staff       (20)     1859 2023-10-26 16:59:37.000000 kelvin-python-sdk-0.0.9/kelvin_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 joaomota   (501) staff       (20)     1087 2023-10-26 16:59:37.000000 kelvin-python-sdk-0.0.9/kelvin_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 joaomota   (501) staff       (20)        1 2023-10-26 16:59:37.000000 kelvin-python-sdk-0.0.9/kelvin_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 joaomota   (501) staff       (20)       64 2023-10-26 16:59:37.000000 kelvin-python-sdk-0.0.9/kelvin_python_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 joaomota   (501) staff       (20)      311 2023-10-26 16:59:37.000000 kelvin-python-sdk-0.0.9/kelvin_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 joaomota   (501) staff       (20)        7 2023-10-26 16:59:37.000000 kelvin-python-sdk-0.0.9/kelvin_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 joaomota   (501) staff       (20)     1881 2023-10-06 12:55:42.000000 kelvin-python-sdk-0.0.9/pyproject.toml
+-rw-r--r--   0 joaomota   (501) staff       (20)       55 2023-10-26 16:54:14.000000 kelvin-python-sdk-0.0.9/requirements.in
+-rw-r--r--   0 joaomota   (501) staff       (20)      761 2023-10-26 16:54:14.000000 kelvin-python-sdk-0.0.9/requirements.txt
+-rw-r--r--   0 joaomota   (501) staff       (20)       38 2023-10-26 16:59:37.215258 kelvin-python-sdk-0.0.9/setup.cfg
+drwxr-xr-x   0 joaomota   (501) staff       (20)        0 2023-10-26 16:59:37.213349 kelvin-python-sdk-0.0.9/tests/
+-rw-r--r--   0 joaomota   (501) staff       (20)     2880 2023-10-20 17:50:42.000000 kelvin-python-sdk-0.0.9/tests/test_client.py
+-rw-r--r--   0 joaomota   (501) staff       (20)     1859 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.9/tests/test_client_calbacks.py
+-rw-r--r--   0 joaomota   (501) staff       (20)      348 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.9/tests/test_filters.py
+-rw-r--r--   0 joaomota   (501) staff       (20)     9089 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.9/tests/test_message.py
+-rw-r--r--   0 joaomota   (501) staff       (20)     1057 2023-10-17 18:16:19.000000 kelvin-python-sdk-0.0.9/tests/test_message_builders.py
+-rw-r--r--   0 joaomota   (501) staff       (20)      407 2023-09-13 18:30:11.000000 kelvin-python-sdk-0.0.9/tests/test_utils.py
+-rw-r--r--   0 joaomota   (501) staff       (20)      652 2023-10-06 12:55:42.000000 kelvin-python-sdk-0.0.9/tox.ini
```

### Comparing `kelvin-python-sdk-0.0.8/.gitignore` & `kelvin-python-sdk-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/Jenkinsfile` & `kelvin-python-sdk-0.0.9/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/PKG-INFO` & `kelvin-python-sdk-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: kelvin-python-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Kelvin Python SDK
 Author-email: Kelvin Inc <engineering@kelvininc.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: arrow==1.2.3
 Requires-Dist: click==8.0.4
 Requires-Dist: pyaml==23.5.8
-Requires-Dist: pydantic==1.10.12
+Requires-Dist: pydantic==1.10.13
+Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: pyyaml==6.0.1
+Requires-Dist: six==1.16.0
 Requires-Dist: structlog==21.5.0
 Requires-Dist: typing-extensions==4.7.1
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-asyncio; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: asyncmock; python_version < "3.8" and extra == "tests"
```

### Comparing `kelvin-python-sdk-0.0.8/README.md` & `kelvin-python-sdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/examples/example.py` & `kelvin-python-sdk-0.0.9/examples/example.py`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/examples/example.yaml` & `kelvin-python-sdk-0.0.9/examples/example.yaml`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/examples/subscriber.py` & `kelvin-python-sdk-0.0.9/examples/subscriber.py`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/kelvin/app/client.py` & `kelvin-python-sdk-0.0.9/kelvin/app/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from __future__ import annotations
 
 import asyncio
 from asyncio import Event, Queue
-from typing import Any, AsyncGenerator, Awaitable, Callable, Optional, Tuple, Union
+from types import TracebackType
+from typing import Any, AsyncGenerator, Awaitable, Callable, Optional, Tuple, Type, TypeVar, Union
 
-from typing_extensions import TypeAlias
+from typing_extensions import Self, TypeAlias
 
 from kelvin.app import filters
 from kelvin.app.config_msg import ConfigMessage
 from kelvin.app.msg_builders import MessageBuilder
 from kelvin.app.stream import KelvinStream, KelvinStreamConfig
 from kelvin.logs import get_logger
 from kelvin.message import KRNAssetParameter, KRNParameter, Message
 
 logger = get_logger(__name__)
 
 NoneCallbackType: TypeAlias = Optional[Callable[..., Awaitable[None]]]
 MessageCallbackType: TypeAlias = Optional[Callable[[Message], Awaitable[None]]]
 
+E = TypeVar("E", bound=Exception)
+
 
 class KelvinApp:
     """Kelvin Client to connect to the Application Stream.
     Use this class to connect and interface with the Kelvin Stream.
 
     After connecting, the connection is handled automatically in the background.
 
@@ -66,14 +69,15 @@
         await self.config_received.wait()
 
     async def disconnect(self) -> None:
         """Disconnects from Kelvin Stream"""
         self._is_to_connect = False
         if self._conn_task:
             await self._conn_task
+        await self._stream.disconnect()
 
     @property
     def asset_parameters(self) -> dict[str, dict[str, Union[bool, float, str]]]:
         """Asset parameters
         A dict containing the parameters of each asset configured to this application.
         eg:
         {
@@ -114,21 +118,35 @@
         sure the configuration is available before continuing.
 
         Returns:
             Event: an awaitable asyncio.Event for the initial app configuration
         """
         return self._config_received
 
-    async def __aenter__(self) -> KelvinApp:
+    async def __aenter__(self) -> Self:
+        """Enter the connection."""
+
         await self.connect()
+
         return self
 
-    async def __aexit__(self, *args: Any) -> bool:
-        await self.disconnect()
-        return True
+    async def __aexit__(
+        self,
+        exc_type: Optional[Type[E]],
+        exc_value: Optional[E],
+        tb: Optional[TracebackType],
+    ) -> Optional[bool]:
+        """Exit the connection."""
+
+        try:
+            await self.disconnect()
+        except Exception:
+            pass
+
+        return None
 
     async def _handle_connection(self) -> None:
         while self._is_to_connect:
             try:
                 try:
                     await self._stream.connect()
                 except ConnectionError:
@@ -171,14 +189,15 @@
 
     def _update_asset_parameter_map(self, asset: str, param: str, value: Any) -> None:
         self._asset_parameters.setdefault(asset, {})[param] = value
 
     def _setup_parameters(self, config_msg: ConfigMessage) -> None:
         for resource in config_msg.payload.resources:
             if resource.type == "asset":
+                self._asset_parameters.setdefault(resource.name, {})  # type: ignore
                 for param, value in resource.parameters.items():
                     self._update_asset_parameter_map(asset=resource.name, param=param, value=value)  # type: ignore
             elif resource.type == "app":
                 for param, value in resource.parameters.items():
                     self._update_app_parameter_map(key=param, value=value)
 
     async def _process_message(self, msg: Message) -> None:
```

### Comparing `kelvin-python-sdk-0.0.8/kelvin/app/config_msg.py` & `kelvin-python-sdk-0.0.9/kelvin/app/config_msg.py`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/kelvin/app/filters.py` & `kelvin-python-sdk-0.0.9/kelvin/app/filters.py`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/kelvin/app/msg_builders.py` & `kelvin-python-sdk-0.0.9/kelvin/app/msg_builders.py`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/kelvin/app/stream.py` & `kelvin-python-sdk-0.0.9/kelvin/app/stream.py`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/kelvin/logs.py` & `kelvin-python-sdk-0.0.9/kelvin/logs.py`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/kelvin/message/__init__.py` & `kelvin-python-sdk-0.0.9/kelvin/message/__init__.py`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/kelvin/message/base_messages.py` & `kelvin-python-sdk-0.0.9/kelvin/message/base_messages.py`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/kelvin/message/krn.py` & `kelvin-python-sdk-0.0.9/kelvin/message/krn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 from typing import Any, Callable, Dict, Generator, Optional, Type
 
+from typing_extensions import Self
+
 
 class KRN:
     """Kelvin Resource Name representation"""
 
     _KRN_TYPES: Dict[str, Type[KRN]] = {}
     _NS_ID: Optional[str] = None
 
@@ -31,29 +33,29 @@
 
         if isinstance(v, KRN):
             return v
 
         raise TypeError("Invalid type for KRN. KRN or string required.")
 
     @classmethod
-    def from_krn(cls, ns_id: str, ns_string: str) -> KRN:
+    def from_krn(cls, ns_id: str, ns_string: str) -> Self:
         return cls(ns_id, ns_string)
 
     @classmethod
-    def from_string(cls, v: str) -> KRN:
+    def from_string(cls, v: str) -> Self:
         try:
             krn, ns_id, ns_string = v.split(":", 2)
         except ValueError:
             raise ValueError("expected format 'krn:<nid>:<nss>'")
 
         if krn != "krn":
             raise ValueError("expected start by 'krn'")
 
         T = KRN._KRN_TYPES.get(ns_id, KRN)
-        return T.from_krn(ns_id, ns_string)
+        return T.from_krn(ns_id, ns_string)  # type: ignore
 
     def __eq__(self, other: Any) -> bool:
         return self.ns_id == other.ns_id and self.ns_string == other.ns_string
 
     def __hash__(self) -> int:
         return hash((self.ns_id, self.ns_string))
 
@@ -76,15 +78,15 @@
         super().__init__(self._NS_ID, asset)
         self.asset = asset
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(asset='{self.asset}')"
 
     @classmethod
-    def from_krn(cls, ns_id: str, ns_string: str) -> KRNAsset:
+    def from_krn(cls, ns_id: str, ns_string: str) -> Self:
         if ns_id != cls._NS_ID:
             raise ValueError(f"Error parsing {cls.__name__}. Expected {cls._NS_ID}, got {ns_id}")
 
         return cls(ns_string)
 
 
 class KRNAssetMetric(KRN):
@@ -98,15 +100,15 @@
         self.asset = asset
         self.metric = metric
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(asset='{self.asset}', metric='{self.metric}')"
 
     @classmethod
-    def from_krn(cls, ns_id: str, ns_string: str) -> KRNAssetMetric:
+    def from_krn(cls, ns_id: str, ns_string: str) -> Self:
         if ns_id != cls._NS_ID:
             raise ValueError(f"Error parsing {cls.__name__}. Expected {cls._NS_ID}, got {ns_id}")
 
         try:
             asset, metric = ns_string.split("/", 1)
         except ValueError:
             raise ValueError("expected format 'krn:am:<asset>/<metric>'")
@@ -125,15 +127,15 @@
         self.asset = asset
         self.data_stream = data_stream
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(asset='{self.asset}', data_stream='{self.data_stream}')"
 
     @classmethod
-    def from_krn(cls, ns_id: str, ns_string: str) -> KRNAssetDataStream:
+    def from_krn(cls, ns_id: str, ns_string: str) -> Self:
         if ns_id != cls._NS_ID:
             raise ValueError(f"Error parsing {cls.__name__}. Expected {cls._NS_ID}, got {ns_id}")
 
         try:
             asset, data_stream = ns_string.split("/", 1)
         except ValueError:
             raise ValueError("expected format 'krn:am:<asset>/<data_stream>'")
@@ -156,15 +158,15 @@
         self.asset = asset
         self.parameter = parameter
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(asset='{self.asset}', parameter='{self.parameter}')"
 
     @classmethod
-    def from_krn(cls, ns_id: str, ns_string: str) -> KRNAssetParameter:
+    def from_krn(cls, ns_id: str, ns_string: str) -> Self:
         if ns_id != cls._NS_ID:
             raise ValueError(f"Error parsing {cls.__name__}. Expected {cls._NS_ID}, got {ns_id}")
 
         try:
             asset, parameter = ns_string.split("/", 1)
         except ValueError:
             raise ValueError("expected format 'krn:am:<asset>/<parameter>'")
@@ -181,15 +183,15 @@
         super().__init__(self._NS_ID, parameter)
         self.parameter = parameter
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(parameter='{self.parameter}')"
 
     @classmethod
-    def from_krn(cls, ns_id: str, ns_string: str) -> KRNParameter:
+    def from_krn(cls, ns_id: str, ns_string: str) -> Self:
         if ns_id != cls._NS_ID:
             raise ValueError(f"Error parsing {cls.__name__}. Expected {cls._NS_ID}, got {ns_id}")
 
         return cls(ns_string)
 
 
 class KRNWorkload(KRN):
@@ -213,15 +215,15 @@
         "Backwards compatibility"
         return self.workload
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(node='{self.node}', workload='{self.workload}')"
 
     @classmethod
-    def from_krn(cls, ns_id: str, ns_string: str) -> KRNWorkload:
+    def from_krn(cls, ns_id: str, ns_string: str) -> Self:
         if ns_id != cls._NS_ID:
             raise ValueError(f"Error parsing {cls.__name__}. Expected {cls._NS_ID}, got {ns_id}")
 
         try:
             node, workload = ns_string.split("/", 1)
         except ValueError:
             raise ValueError("expected format 'krn:wl:<node>/<workload>'")
@@ -252,15 +254,15 @@
         "Backwards compatibility"
         return self.workload
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(node='{self.node}', workload='{self.workload}', app='{self.app}')"
 
     @classmethod
-    def from_krn(cls, ns_id: str, ns_string: str) -> KRNWorkloadApp:
+    def from_krn(cls, ns_id: str, ns_string: str) -> Self:
         if ns_id != cls._NS_ID:
             raise ValueError(f"Error parsing {cls.__name__}. Expected {cls._NS_ID}, got {ns_id}")
 
         try:
             node_workload, app = ns_string.split(":", 1)
             node, workload = node_workload.split("/", 1)
         except ValueError:
@@ -278,12 +280,12 @@
         super().__init__(self._NS_ID, recommendation_id)
         self.recommendation_id = recommendation_id
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(recommendation_id='{self.recommendation_id}')"
 
     @classmethod
-    def from_krn(cls, ns_id: str, ns_string: str) -> KRNRecommendation:
+    def from_krn(cls, ns_id: str, ns_string: str) -> Self:
         if ns_id != cls._NS_ID:
             raise ValueError(f"Error parsing {cls.__name__}. Expected {cls._NS_ID}, got {ns_id}")
 
         return cls(ns_string)
```

### Comparing `kelvin-python-sdk-0.0.8/kelvin/message/message.py` & `kelvin-python-sdk-0.0.9/kelvin/message/message.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,37 +2,34 @@
 
 from datetime import datetime
 from functools import wraps
 from typing import Any, ClassVar, Dict, Optional, Type, Union
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel, Field, validator
+from typing_extensions import Self
 
-from kelvin.logs import get_logger
 from kelvin.message.krn import KRN, KRNAssetDataStream
 from kelvin.message.msg_type import KMessageType, KMessageTypeData, KMessageTypePrimitive
 from kelvin.message.utils import from_rfc3339_timestamp, to_rfc3339_timestamp
 
-logger = get_logger(__name__)
-
-
 # Set to True to fail when parsing unknown message types
 FAIL_ON_UNKNOWN_TYPES = False
 
 
 class Message(BaseModel):
     _MESSAGE_TYPES: ClassVar[Dict[KMessageType, Type["Message"]]] = {}
     _TYPE: ClassVar[Optional[KMessageType]] = None
 
     id: UUID = Field(default_factory=lambda: uuid4())
     type: Optional[KMessageType] = None
     trace_id: Optional[str] = None
     source: Optional[KRN] = None
     timestamp: datetime = Field(default_factory=lambda: datetime.now().astimezone())
-    resource: Optional[KRN]
+    resource: Optional[KRN] = None
 
     payload: Any
 
     class Config:
         underscore_attrs_are_private = True
         json_encoders = {
             datetime: to_rfc3339_timestamp,
@@ -123,15 +120,15 @@
         return super().json(by_alias=by_alias, exclude_none=exclude_none, exclude_unset=exclude_unset, **kwargs)
 
     def encode(self) -> bytes:
         """Encode message"""
         return bytes(self.json(), "utf-8")
 
     @classmethod
-    def decode(cls, data: bytes) -> Message:
+    def decode(cls, data: bytes) -> Self:
         return cls.parse_raw(data)
 
     @staticmethod
     def _convert_message_v1(**kwargs: Dict) -> Dict:
         result: Dict[str, Any] = {
             "id": kwargs.get("id", None),
             "timestamp": kwargs.get("timestamp", None),
```

### Comparing `kelvin-python-sdk-0.0.8/kelvin/message/msg_type.py` & `kelvin-python-sdk-0.0.9/kelvin/message/msg_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, Callable, Dict, Generator, Optional, Type
 
+from typing_extensions import Self
+
 
 class KMessageType:
     """Kelvin Message Type representation"""
 
     _SUBTYPES: Dict[str, Type[KMessageType]] = {}
     _TYPE: str = ""
 
@@ -26,42 +28,42 @@
         yield cls.validate
 
     @classmethod
     def validate(cls, v: Any) -> KMessageType:
         if isinstance(v, str):
             return cls.from_string(v)
 
-        if isinstance(v, KMessageType):
+        if isinstance(v, cls):
             return v
 
         raise TypeError("Invalid type for KMessageType. KMessageType or string required.")
 
     @classmethod
     def from_krn(cls, msg_type: str, components: Dict[str, str]) -> KMessageType:
         T = KMessageType._SUBTYPES.get(msg_type, None)
         if T is not None:
             return T.from_krn(msg_type, components)
 
         return cls(msg_type, components)
 
     @classmethod
-    def from_string(cls, v: str) -> KMessageType:
+    def from_string(cls, v: str) -> Self:
         if not isinstance(v, str):
             raise TypeError("string required")
 
         msg_type, *components = v.split(";")
         components_dict = {}
         for component in components:
             try:
                 key, value = component.split("=", 1)
             except ValueError:
                 raise ValueError(f"Invalid type '{v}'. Expected format '<type>;<key>=<value>'")
             components_dict[key] = value
 
-        return cls.from_krn(msg_type, components_dict)
+        return cls.from_krn(msg_type, components_dict)  # type: ignore
 
     def __eq__(self, other: Any) -> bool:
         if type(self) is not type(other):
             return False
 
         return self.msg_type == other.msg_type and self.components == other.components
 
@@ -95,15 +97,15 @@
         if icd is not None:
             components["icd"] = icd
         super().__init__(self._TYPE, components)
         self.primitive = PrimitiveTypes[primitive]
         self.icd = icd
 
     @classmethod
-    def from_krn(cls, msg_type: str, components: Optional[Dict[str, str]]) -> KMessageTypePrimitive:
+    def from_krn(cls, msg_type: str, components: Optional[Dict[str, str]]) -> Self:
         if msg_type != cls._TYPE:
             raise ValueError(f"Error parsing {cls.__name__}. Expected {cls._TYPE}, got {msg_type}")
 
         primitive = components.get("pt", "object") if components else "object"
         icd = components.get("icd", None) if components else None
 
         return cls(primitive, icd)  # type: ignore
@@ -123,25 +125,25 @@
     _TYPE = "parameter"
 
 
 class KMessageTypeControl(KMessageType):
     _TYPE = "control"
 
     @classmethod
-    def from_krn(cls, _: str, __: Optional[Dict[str, str]]) -> KMessageTypeControl:
+    def from_krn(cls, _: str, __: Optional[Dict[str, str]]) -> Self:
         return cls(cls._TYPE, {})
 
 
 class KMessageTypeControlStatus(KMessageType):
     _TYPE = "control-status"
 
     @classmethod
-    def from_krn(cls, _: str, __: Optional[Dict[str, str]]) -> KMessageTypeControlStatus:
+    def from_krn(cls, _: str, __: Optional[Dict[str, str]]) -> Self:
         return cls(cls._TYPE)
 
 
 class KMessageTypeRecommendation(KMessageType):
     _TYPE = "recommendation"
 
     @classmethod
-    def from_krn(cls, _: str, __: Optional[Dict[str, str]]) -> KMessageTypeRecommendation:
+    def from_krn(cls, _: str, __: Optional[Dict[str, str]]) -> Self:
         return cls(cls._TYPE)
```

### Comparing `kelvin-python-sdk-0.0.8/kelvin/message/primitives.py` & `kelvin-python-sdk-0.0.9/kelvin/message/primitives.py`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/kelvin/message/utils.py` & `kelvin-python-sdk-0.0.9/kelvin/message/utils.py`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/kelvin/publisher/config.py` & `kelvin-python-sdk-0.0.9/kelvin/publisher/config.py`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/kelvin_python_sdk.egg-info/PKG-INFO` & `kelvin-python-sdk-0.0.9/kelvin_python_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: kelvin-python-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Kelvin Python SDK
 Author-email: Kelvin Inc <engineering@kelvininc.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: arrow==1.2.3
 Requires-Dist: click==8.0.4
 Requires-Dist: pyaml==23.5.8
-Requires-Dist: pydantic==1.10.12
+Requires-Dist: pydantic==1.10.13
+Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: pyyaml==6.0.1
+Requires-Dist: six==1.16.0
 Requires-Dist: structlog==21.5.0
 Requires-Dist: typing-extensions==4.7.1
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-asyncio; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: asyncmock; python_version < "3.8" and extra == "tests"
```

### Comparing `kelvin-python-sdk-0.0.8/kelvin_python_sdk.egg-info/SOURCES.txt` & `kelvin-python-sdk-0.0.9/kelvin_python_sdk.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 pyproject.toml
 requirements.in
 requirements.txt
 tox.ini
 examples/example.py
 examples/example.yaml
 examples/subscriber.py
+examples/csv/csv_app.py
+examples/csv/csv_app.yaml
+examples/csv/data.csv
 kelvin/logs.py
 kelvin/app/__init__.py
 kelvin/app/client.py
 kelvin/app/config_msg.py
 kelvin/app/filters.py
 kelvin/app/msg_builders.py
 kelvin/app/stream.py
```

### Comparing `kelvin-python-sdk-0.0.8/pyproject.toml` & `kelvin-python-sdk-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/requirements.txt` & `kelvin-python-sdk-0.0.9/requirements.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --constraint=constraints.txt --no-emit-index-url --output-file=requirements.txt --pre requirements.in
 #
+arrow==1.2.3
+    # via
+    #   -c constraints.txt
+    #   -r requirements.in
 click==8.0.4
     # via
     #   -c constraints.txt
     #   -r requirements.in
 pyaml==23.5.8
     # via -r requirements.in
-pydantic==1.10.12
+pydantic==1.10.13
     # via
     #   -c constraints.txt
     #   -r requirements.in
+python-dateutil==2.8.2
+    # via arrow
 pyyaml==6.0.1
     # via
     #   -c constraints.txt
     #   pyaml
+six==1.16.0
+    # via python-dateutil
 structlog==21.5.0
     # via
     #   -c constraints.txt
     #   -r requirements.in
 typing-extensions==4.7.1
     # via pydantic
```

### Comparing `kelvin-python-sdk-0.0.8/tests/test_client.py` & `kelvin-python-sdk-0.0.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/tests/test_client_calbacks.py` & `kelvin-python-sdk-0.0.9/tests/test_client_calbacks.py`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/tests/test_message.py` & `kelvin-python-sdk-0.0.9/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/tests/test_message_builders.py` & `kelvin-python-sdk-0.0.9/tests/test_message_builders.py`

 * *Files identical despite different names*

### Comparing `kelvin-python-sdk-0.0.8/tox.ini` & `kelvin-python-sdk-0.0.9/tox.ini`

 * *Files identical despite different names*

