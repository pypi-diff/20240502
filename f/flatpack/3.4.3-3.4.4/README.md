# Comparing `tmp/flatpack-3.4.3.tar.gz` & `tmp/flatpack-3.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.4.3.tar", last modified: Thu May  2 08:12:10 2024, max compression
+gzip compressed data, was "flatpack-3.4.4.tar", last modified: Thu May  2 08:16:52 2024, max compression
```

## Comparing `flatpack-3.4.3.tar` & `flatpack-3.4.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 08:12:10.134979 flatpack-3.4.3/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.3/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 08:12:10.134658 flatpack-3.4.3/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-01 14:25:58.000000 flatpack-3.4.3/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 08:12:10.130750 flatpack-3.4.3/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      111 2024-04-27 22:37:06.000000 flatpack-3.4.3/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.3/flatpack/agent_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.3/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.3/flatpack/datasets.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 08:12:10.132670 flatpack-3.4.3/flatpack/engines/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.3/flatpack/engines/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1137 2024-05-02 08:03:32.000000 flatpack-3.4.3/flatpack/engines/engine_llama_cpp.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1256 2024-05-02 08:12:00.000000 flatpack-3.4.3/flatpack/engines/fast_api_test.py
--rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.3/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.3/flatpack/load_modules.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    26214 2024-04-29 21:37:50.000000 flatpack-3.4.3/flatpack/main.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 08:12:10.133837 flatpack-3.4.3/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.3/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.3/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.3/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6876 2024-04-27 20:15:24.000000 flatpack-3.4.3/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.3/flatpack/session_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.3/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6413 2024-04-27 15:03:11.000000 flatpack-3.4.3/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 08:12:10.134222 flatpack-3.4.3/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 08:12:10.000000 flatpack-3.4.3/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      645 2024-05-02 08:12:10.000000 flatpack-3.4.3/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-02 08:12:10.000000 flatpack-3.4.3/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-02 08:12:10.000000 flatpack-3.4.3/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-02 08:12:10.000000 flatpack-3.4.3/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-02 08:12:10.000000 flatpack-3.4.3/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-02 08:12:10.135048 flatpack-3.4.3/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)     1089 2024-05-02 07:30:40.000000 flatpack-3.4.3/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 08:16:52.514761 flatpack-3.4.4/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.4/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 08:16:52.514387 flatpack-3.4.4/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-01 14:25:58.000000 flatpack-3.4.4/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 08:16:52.510918 flatpack-3.4.4/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      111 2024-04-27 22:37:06.000000 flatpack-3.4.4/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.4/flatpack/agent_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.4/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.4/flatpack/datasets.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 08:16:52.512667 flatpack-3.4.4/flatpack/engines/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.4/flatpack/engines/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1137 2024-05-02 08:03:32.000000 flatpack-3.4.4/flatpack/engines/engine_llama_cpp.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1256 2024-05-02 08:12:00.000000 flatpack-3.4.4/flatpack/engines/fast_api_test.py
+-rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.4/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.4/flatpack/load_modules.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    26214 2024-04-29 21:37:50.000000 flatpack-3.4.4/flatpack/main.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 08:16:52.513390 flatpack-3.4.4/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.4/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.4/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.4/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6876 2024-04-27 20:15:24.000000 flatpack-3.4.4/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.4/flatpack/session_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.4/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6413 2024-04-27 15:03:11.000000 flatpack-3.4.4/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 08:16:52.513730 flatpack-3.4.4/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 08:16:52.000000 flatpack-3.4.4/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      645 2024-05-02 08:16:52.000000 flatpack-3.4.4/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-02 08:16:52.000000 flatpack-3.4.4/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-02 08:16:52.000000 flatpack-3.4.4/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-02 08:16:52.000000 flatpack-3.4.4/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-02 08:16:52.000000 flatpack-3.4.4/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-02 08:16:52.514826 flatpack-3.4.4/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1089 2024-05-02 08:13:19.000000 flatpack-3.4.4/setup.py
```

### Comparing `flatpack-3.4.3/LICENSE` & `flatpack-3.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.3/PKG-INFO` & `flatpack-3.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.3
+Version: 3.4.4
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.4.3/README.md` & `flatpack-3.4.4/README.md`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.3/flatpack/agent_manager.py` & `flatpack-3.4.4/flatpack/agent_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.3/flatpack/datasets.py` & `flatpack-3.4.4/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.3/flatpack/engines/engine_llama_cpp.py` & `flatpack-3.4.4/flatpack/engines/engine_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.3/flatpack/engines/fast_api_test.py` & `flatpack-3.4.4/flatpack/engines/fast_api_test.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.3/flatpack/instructions.py` & `flatpack-3.4.4/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.3/flatpack/main.py` & `flatpack-3.4.4/flatpack/main.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.3/flatpack/modules/lstm.py` & `flatpack-3.4.4/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.3/flatpack/modules/rnn.py` & `flatpack-3.4.4/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.3/flatpack/parsers.py` & `flatpack-3.4.4/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.3/flatpack/vector_manager.py` & `flatpack-3.4.4/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.3/flatpack.egg-info/PKG-INFO` & `flatpack-3.4.4/flatpack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.3
+Version: 3.4.4
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.4.3/flatpack.egg-info/SOURCES.txt` & `flatpack-3.4.4/flatpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.3/setup.py` & `flatpack-3.4.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.4.3",
+    version="3.4.4",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.5",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.2",
```

