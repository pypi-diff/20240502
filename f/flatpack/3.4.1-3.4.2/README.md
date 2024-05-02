# Comparing `tmp/flatpack-3.4.1.tar.gz` & `tmp/flatpack-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.4.1.tar", last modified: Wed May  1 14:27:37 2024, max compression
+gzip compressed data, was "flatpack-3.4.2.tar", last modified: Thu May  2 07:16:40 2024, max compression
```

## Comparing `flatpack-3.4.1.tar` & `flatpack-3.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-01 14:27:37.908445 flatpack-3.4.1/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.1/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-01 14:27:37.908256 flatpack-3.4.1/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-01 14:25:58.000000 flatpack-3.4.1/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-01 14:27:37.905888 flatpack-3.4.1/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      111 2024-04-27 22:37:06.000000 flatpack-3.4.1/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2547 2024-05-01 07:51:50.000000 flatpack-3.4.1/flatpack/agent_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.1/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.1/flatpack/datasets.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-01 14:27:37.907175 flatpack-3.4.1/flatpack/engines/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.1/flatpack/engines/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      796 2024-04-29 23:15:22.000000 flatpack-3.4.1/flatpack/engines/engine_llama_cpp.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      922 2024-04-29 23:48:47.000000 flatpack-3.4.1/flatpack/engines/fast_api_test.py
--rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.1/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.1/flatpack/load_modules.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    26214 2024-04-29 21:37:50.000000 flatpack-3.4.1/flatpack/main.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-01 14:27:37.907779 flatpack-3.4.1/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.1/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.1/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.1/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6876 2024-04-27 20:15:24.000000 flatpack-3.4.1/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.1/flatpack/session_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.1/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6413 2024-04-27 15:03:11.000000 flatpack-3.4.1/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-01 14:27:37.908031 flatpack-3.4.1/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-01 14:27:37.000000 flatpack-3.4.1/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      645 2024-05-01 14:27:37.000000 flatpack-3.4.1/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-01 14:27:37.000000 flatpack-3.4.1/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-01 14:27:37.000000 flatpack-3.4.1/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-01 14:27:37.000000 flatpack-3.4.1/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-01 14:27:37.000000 flatpack-3.4.1/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-01 14:27:37.908492 flatpack-3.4.1/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)     1089 2024-05-01 14:20:49.000000 flatpack-3.4.1/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 07:16:40.187330 flatpack-3.4.2/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.2/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 07:16:40.187031 flatpack-3.4.2/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-01 14:25:58.000000 flatpack-3.4.2/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 07:16:40.184187 flatpack-3.4.2/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      111 2024-04-27 22:37:06.000000 flatpack-3.4.2/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     2547 2024-05-01 07:51:50.000000 flatpack-3.4.2/flatpack/agent_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.2/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.2/flatpack/datasets.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 07:16:40.185737 flatpack-3.4.2/flatpack/engines/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.2/flatpack/engines/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      796 2024-04-29 23:15:22.000000 flatpack-3.4.2/flatpack/engines/engine_llama_cpp.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1259 2024-05-01 15:34:17.000000 flatpack-3.4.2/flatpack/engines/fast_api_test.py
+-rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.2/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.2/flatpack/load_modules.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    26214 2024-04-29 21:37:50.000000 flatpack-3.4.2/flatpack/main.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 07:16:40.186257 flatpack-3.4.2/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.2/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.2/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.2/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6876 2024-04-27 20:15:24.000000 flatpack-3.4.2/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.2/flatpack/session_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.2/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6413 2024-04-27 15:03:11.000000 flatpack-3.4.2/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 07:16:40.186659 flatpack-3.4.2/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 07:16:40.000000 flatpack-3.4.2/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      645 2024-05-02 07:16:40.000000 flatpack-3.4.2/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-02 07:16:40.000000 flatpack-3.4.2/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-02 07:16:40.000000 flatpack-3.4.2/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-02 07:16:40.000000 flatpack-3.4.2/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-02 07:16:40.000000 flatpack-3.4.2/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-02 07:16:40.187399 flatpack-3.4.2/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1089 2024-05-01 14:42:33.000000 flatpack-3.4.2/setup.py
```

### Comparing `flatpack-3.4.1/LICENSE` & `flatpack-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.1/PKG-INFO` & `flatpack-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.1
+Version: 3.4.2
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.4.1/README.md` & `flatpack-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.1/flatpack/agent_manager.py` & `flatpack-3.4.2/flatpack/agent_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.1/flatpack/datasets.py` & `flatpack-3.4.2/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.1/flatpack/engines/engine_llama_cpp.py` & `flatpack-3.4.2/flatpack/engines/engine_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.1/flatpack/engines/fast_api_test.py` & `flatpack-3.4.2/flatpack/engines/fast_api_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 import os
 import uvicorn
 
 from fastapi import FastAPI, HTTPException
-from engine_llama_cpp import LlamaCPPEngine
 from pydantic import BaseModel
 
 app = FastAPI()
 
-engine = LlamaCPPEngine(
-    repo_id="microsoft/Phi-3-mini-4k-instruct-gguf",
-    filename="*q4.gguf",
-    n_ctx=4096,
-    n_threads=8,
-    verbose=False
-)
+
+class LlamaEngineSingleton:
+    engine_instance = None
+
+    @classmethod
+    def get_instance(cls):
+        from engine_llama_cpp import LlamaCPPEngine
+        if cls.engine_engine_instance is None:
+            cls.engine_instance = LlamaCPPEngine(
+                repo_id="microsoft/Phi-3-mini-4k-instruct-gguf",
+                filename="*q4.gguf",
+                n_ctx=4096,
+                n_threads=8,
+                verbose=False
+            )
+        return cls.engine_instance
 
 
 class Query(BaseModel):
     context: str
     question: str
 
 
 @app.post("/generate-response/")
 async def generate_response(query: Query):
+    engine = LlamaEngineSingleton.get_instance()
     try:
         response = engine.generate_response(context=query.context, question=query.question)
         return {"response": response}
     except Exception as e:
         raise HTTPException(status_code=500, detail=str(e))
```

### Comparing `flatpack-3.4.1/flatpack/instructions.py` & `flatpack-3.4.2/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.1/flatpack/main.py` & `flatpack-3.4.2/flatpack/main.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.1/flatpack/modules/lstm.py` & `flatpack-3.4.2/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.1/flatpack/modules/rnn.py` & `flatpack-3.4.2/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.1/flatpack/parsers.py` & `flatpack-3.4.2/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.1/flatpack/vector_manager.py` & `flatpack-3.4.2/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.1/flatpack.egg-info/PKG-INFO` & `flatpack-3.4.2/flatpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.1
+Version: 3.4.2
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.4.1/flatpack.egg-info/SOURCES.txt` & `flatpack-3.4.2/flatpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.1/setup.py` & `flatpack-3.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.4.1",
+    version="3.4.2",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.5",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.2",
```

