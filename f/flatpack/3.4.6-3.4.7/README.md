# Comparing `tmp/flatpack-3.4.6.tar.gz` & `tmp/flatpack-3.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.4.6.tar", last modified: Thu May  2 10:07:00 2024, max compression
+gzip compressed data, was "flatpack-3.4.7.tar", last modified: Thu May  2 14:43:57 2024, max compression
```

## Comparing `flatpack-3.4.6.tar` & `flatpack-3.4.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 10:07:00.811749 flatpack-3.4.6/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.6/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 10:07:00.811564 flatpack-3.4.6/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-01 14:25:58.000000 flatpack-3.4.6/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 10:07:00.808968 flatpack-3.4.6/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      111 2024-04-27 22:37:06.000000 flatpack-3.4.6/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.6/flatpack/agent_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.6/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.6/flatpack/datasets.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 10:07:00.810405 flatpack-3.4.6/flatpack/engines/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.6/flatpack/engines/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      796 2024-05-02 08:44:24.000000 flatpack-3.4.6/flatpack/engines/engine_llama_cpp.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      922 2024-05-02 08:44:56.000000 flatpack-3.4.6/flatpack/engines/fast_api_test.py
--rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.6/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.6/flatpack/load_modules.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    26234 2024-05-02 10:00:01.000000 flatpack-3.4.6/flatpack/main.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 10:07:00.811087 flatpack-3.4.6/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.6/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.6/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.6/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6876 2024-04-27 20:15:24.000000 flatpack-3.4.6/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.6/flatpack/session_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.6/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6413 2024-04-27 15:03:11.000000 flatpack-3.4.6/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 10:07:00.811333 flatpack-3.4.6/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 10:07:00.000000 flatpack-3.4.6/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      645 2024-05-02 10:07:00.000000 flatpack-3.4.6/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-02 10:07:00.000000 flatpack-3.4.6/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-02 10:07:00.000000 flatpack-3.4.6/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-02 10:07:00.000000 flatpack-3.4.6/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-02 10:07:00.000000 flatpack-3.4.6/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-02 10:07:00.811790 flatpack-3.4.6/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)     1089 2024-05-02 09:57:31.000000 flatpack-3.4.6/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:43:57.305091 flatpack-3.4.7/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.7/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 14:43:57.304801 flatpack-3.4.7/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-01 14:25:58.000000 flatpack-3.4.7/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:43:57.301780 flatpack-3.4.7/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.4.7/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.7/flatpack/agent_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.7/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.7/flatpack/datasets.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:43:57.303219 flatpack-3.4.7/flatpack/engines/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.7/flatpack/engines/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      796 2024-05-02 08:44:24.000000 flatpack-3.4.7/flatpack/engines/engine_llama_cpp.py
+-rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.7/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-02 14:38:54.000000 flatpack-3.4.7/flatpack/load_engines.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.7/flatpack/load_modules.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    26234 2024-05-02 10:00:01.000000 flatpack-3.4.7/flatpack/main.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:43:57.304016 flatpack-3.4.7/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.7/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.7/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.7/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6876 2024-04-27 20:15:24.000000 flatpack-3.4.7/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.7/flatpack/session_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.7/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6413 2024-04-27 15:03:11.000000 flatpack-3.4.7/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:43:57.304406 flatpack-3.4.7/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 14:43:57.000000 flatpack-3.4.7/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-02 14:43:57.000000 flatpack-3.4.7/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-02 14:43:57.000000 flatpack-3.4.7/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-02 14:43:57.000000 flatpack-3.4.7/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-02 14:43:57.000000 flatpack-3.4.7/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-02 14:43:57.000000 flatpack-3.4.7/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-02 14:43:57.305164 flatpack-3.4.7/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1089 2024-05-02 14:31:49.000000 flatpack-3.4.7/setup.py
```

### Comparing `flatpack-3.4.6/LICENSE` & `flatpack-3.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.6/PKG-INFO` & `flatpack-3.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.6
+Version: 3.4.7
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.4.6/README.md` & `flatpack-3.4.7/README.md`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.6/flatpack/agent_manager.py` & `flatpack-3.4.7/flatpack/agent_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.6/flatpack/datasets.py` & `flatpack-3.4.7/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.6/flatpack/engines/engine_llama_cpp.py` & `flatpack-3.4.7/flatpack/engines/engine_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.6/flatpack/instructions.py` & `flatpack-3.4.7/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.6/flatpack/main.py` & `flatpack-3.4.7/flatpack/main.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.6/flatpack/modules/lstm.py` & `flatpack-3.4.7/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.6/flatpack/modules/rnn.py` & `flatpack-3.4.7/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.6/flatpack/parsers.py` & `flatpack-3.4.7/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.6/flatpack/vector_manager.py` & `flatpack-3.4.7/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.6/flatpack.egg-info/PKG-INFO` & `flatpack-3.4.7/flatpack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.6
+Version: 3.4.7
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.4.6/flatpack.egg-info/SOURCES.txt` & `flatpack-3.4.7/flatpack.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 README.md
 setup.py
 flatpack/__init__.py
 flatpack/agent_manager.py
 flatpack/config.py
 flatpack/datasets.py
 flatpack/instructions.py
+flatpack/load_engines.py
 flatpack/load_modules.py
 flatpack/main.py
 flatpack/parsers.py
 flatpack/session_manager.py
 flatpack/utils.py
 flatpack/vector_manager.py
 flatpack.egg-info/PKG-INFO
 flatpack.egg-info/SOURCES.txt
 flatpack.egg-info/dependency_links.txt
 flatpack.egg-info/entry_points.txt
 flatpack.egg-info/requires.txt
 flatpack.egg-info/top_level.txt
 flatpack/engines/__init__.py
 flatpack/engines/engine_llama_cpp.py
-flatpack/engines/fast_api_test.py
 flatpack/modules/__init__.py
 flatpack/modules/lstm.py
 flatpack/modules/rnn.py
```

### Comparing `flatpack-3.4.6/setup.py` & `flatpack-3.4.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.4.6",
+    version="3.4.7",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.5",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.2",
```

