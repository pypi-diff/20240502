# Comparing `tmp/flatpack-3.4.2.tar.gz` & `tmp/flatpack-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.4.2.tar", last modified: Thu May  2 07:16:40 2024, max compression
+gzip compressed data, was "flatpack-3.4.3.tar", last modified: Thu May  2 08:12:10 2024, max compression
```

## Comparing `flatpack-3.4.2.tar` & `flatpack-3.4.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 07:16:40.187330 flatpack-3.4.2/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.2/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 07:16:40.187031 flatpack-3.4.2/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-01 14:25:58.000000 flatpack-3.4.2/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 07:16:40.184187 flatpack-3.4.2/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      111 2024-04-27 22:37:06.000000 flatpack-3.4.2/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2547 2024-05-01 07:51:50.000000 flatpack-3.4.2/flatpack/agent_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.2/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.2/flatpack/datasets.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 07:16:40.185737 flatpack-3.4.2/flatpack/engines/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.2/flatpack/engines/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      796 2024-04-29 23:15:22.000000 flatpack-3.4.2/flatpack/engines/engine_llama_cpp.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1259 2024-05-01 15:34:17.000000 flatpack-3.4.2/flatpack/engines/fast_api_test.py
--rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.2/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.2/flatpack/load_modules.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    26214 2024-04-29 21:37:50.000000 flatpack-3.4.2/flatpack/main.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 07:16:40.186257 flatpack-3.4.2/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.2/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.2/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.2/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6876 2024-04-27 20:15:24.000000 flatpack-3.4.2/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.2/flatpack/session_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.2/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6413 2024-04-27 15:03:11.000000 flatpack-3.4.2/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 07:16:40.186659 flatpack-3.4.2/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 07:16:40.000000 flatpack-3.4.2/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      645 2024-05-02 07:16:40.000000 flatpack-3.4.2/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-02 07:16:40.000000 flatpack-3.4.2/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-02 07:16:40.000000 flatpack-3.4.2/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-02 07:16:40.000000 flatpack-3.4.2/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-02 07:16:40.000000 flatpack-3.4.2/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-02 07:16:40.187399 flatpack-3.4.2/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)     1089 2024-05-01 14:42:33.000000 flatpack-3.4.2/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 08:12:10.134979 flatpack-3.4.3/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.3/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 08:12:10.134658 flatpack-3.4.3/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-01 14:25:58.000000 flatpack-3.4.3/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 08:12:10.130750 flatpack-3.4.3/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      111 2024-04-27 22:37:06.000000 flatpack-3.4.3/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.3/flatpack/agent_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.3/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.3/flatpack/datasets.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 08:12:10.132670 flatpack-3.4.3/flatpack/engines/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.3/flatpack/engines/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1137 2024-05-02 08:03:32.000000 flatpack-3.4.3/flatpack/engines/engine_llama_cpp.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1256 2024-05-02 08:12:00.000000 flatpack-3.4.3/flatpack/engines/fast_api_test.py
+-rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.3/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.3/flatpack/load_modules.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    26214 2024-04-29 21:37:50.000000 flatpack-3.4.3/flatpack/main.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 08:12:10.133837 flatpack-3.4.3/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.3/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.3/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.3/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6876 2024-04-27 20:15:24.000000 flatpack-3.4.3/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.3/flatpack/session_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.3/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6413 2024-04-27 15:03:11.000000 flatpack-3.4.3/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 08:12:10.134222 flatpack-3.4.3/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 08:12:10.000000 flatpack-3.4.3/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      645 2024-05-02 08:12:10.000000 flatpack-3.4.3/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-02 08:12:10.000000 flatpack-3.4.3/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-02 08:12:10.000000 flatpack-3.4.3/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-02 08:12:10.000000 flatpack-3.4.3/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-02 08:12:10.000000 flatpack-3.4.3/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-02 08:12:10.135048 flatpack-3.4.3/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1089 2024-05-02 07:30:40.000000 flatpack-3.4.3/setup.py
```

### Comparing `flatpack-3.4.2/LICENSE` & `flatpack-3.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.2/PKG-INFO` & `flatpack-3.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.2
+Version: 3.4.3
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.4.2/README.md` & `flatpack-3.4.3/README.md`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.2/flatpack/agent_manager.py` & `flatpack-3.4.3/flatpack/agent_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import psutil
 import signal
 import socket
 import subprocess
 
 from datetime import datetime
-from .engines.engine_llama_cpp import LlamaCPPEngine
 from pathlib import Path
 
 
 def find_free_port():
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
         s.bind(('', 0))
         s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
```

### Comparing `flatpack-3.4.2/flatpack/datasets.py` & `flatpack-3.4.3/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.2/flatpack/engines/fast_api_test.py` & `flatpack-3.4.3/flatpack/engines/fast_api_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 
 class LlamaEngineSingleton:
     engine_instance = None
 
     @classmethod
     def get_instance(cls):
-        from engine_llama_cpp import LlamaCPPEngine
-        if cls.engine_engine_instance is None:
+        if cls.engine_instance is None:
+            from engine_llama_cpp import LlamaCPPEngine
             cls.engine_instance = LlamaCPPEngine(
                 repo_id="microsoft/Phi-3-mini-4k-instruct-gguf",
                 filename="*q4.gguf",
                 n_ctx=4096,
                 n_threads=8,
                 verbose=False
             )
```

### Comparing `flatpack-3.4.2/flatpack/instructions.py` & `flatpack-3.4.3/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.2/flatpack/main.py` & `flatpack-3.4.3/flatpack/main.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.2/flatpack/modules/lstm.py` & `flatpack-3.4.3/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.2/flatpack/modules/rnn.py` & `flatpack-3.4.3/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.2/flatpack/parsers.py` & `flatpack-3.4.3/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.2/flatpack/vector_manager.py` & `flatpack-3.4.3/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.2/flatpack.egg-info/PKG-INFO` & `flatpack-3.4.3/flatpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.2
+Version: 3.4.3
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.4.2/flatpack.egg-info/SOURCES.txt` & `flatpack-3.4.3/flatpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.2/setup.py` & `flatpack-3.4.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.4.2",
+    version="3.4.3",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.5",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.2",
```

