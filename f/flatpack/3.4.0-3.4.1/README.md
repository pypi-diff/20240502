# Comparing `tmp/flatpack-3.4.0.tar.gz` & `tmp/flatpack-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.4.0.tar", last modified: Mon Apr 29 23:57:17 2024, max compression
+gzip compressed data, was "flatpack-3.4.1.tar", last modified: Wed May  1 14:27:37 2024, max compression
```

## Comparing `flatpack-3.4.0.tar` & `flatpack-3.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:57:17.373623 flatpack-3.4.0/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.0/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     6084 2024-04-29 23:57:17.373352 flatpack-3.4.0/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5285 2024-04-29 23:56:39.000000 flatpack-3.4.0/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:57:17.370198 flatpack-3.4.0/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      111 2024-04-27 22:37:06.000000 flatpack-3.4.0/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2836 2024-04-29 23:48:33.000000 flatpack-3.4.0/flatpack/agent_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.0/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.0/flatpack/datasets.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:57:17.371927 flatpack-3.4.0/flatpack/engines/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.0/flatpack/engines/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      796 2024-04-29 23:15:22.000000 flatpack-3.4.0/flatpack/engines/engine_llama_cpp.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      922 2024-04-29 23:48:47.000000 flatpack-3.4.0/flatpack/engines/fast_api_test.py
--rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.0/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.0/flatpack/load_modules.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    26214 2024-04-29 21:37:50.000000 flatpack-3.4.0/flatpack/main.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:57:17.372725 flatpack-3.4.0/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.0/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.0/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.0/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6876 2024-04-27 20:15:24.000000 flatpack-3.4.0/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.0/flatpack/session_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.0/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6413 2024-04-27 15:03:11.000000 flatpack-3.4.0/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:57:17.373041 flatpack-3.4.0/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     6084 2024-04-29 23:57:17.000000 flatpack-3.4.0/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      645 2024-04-29 23:57:17.000000 flatpack-3.4.0/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-04-29 23:57:17.000000 flatpack-3.4.0/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-04-29 23:57:17.000000 flatpack-3.4.0/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      297 2024-04-29 23:57:17.000000 flatpack-3.4.0/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-04-29 23:57:17.000000 flatpack-3.4.0/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-04-29 23:57:17.373681 flatpack-3.4.0/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)     1062 2024-04-29 23:56:48.000000 flatpack-3.4.0/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-01 14:27:37.908445 flatpack-3.4.1/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.1/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-01 14:27:37.908256 flatpack-3.4.1/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-01 14:25:58.000000 flatpack-3.4.1/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-01 14:27:37.905888 flatpack-3.4.1/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      111 2024-04-27 22:37:06.000000 flatpack-3.4.1/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     2547 2024-05-01 07:51:50.000000 flatpack-3.4.1/flatpack/agent_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.1/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.1/flatpack/datasets.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-01 14:27:37.907175 flatpack-3.4.1/flatpack/engines/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.1/flatpack/engines/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      796 2024-04-29 23:15:22.000000 flatpack-3.4.1/flatpack/engines/engine_llama_cpp.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      922 2024-04-29 23:48:47.000000 flatpack-3.4.1/flatpack/engines/fast_api_test.py
+-rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.1/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.1/flatpack/load_modules.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    26214 2024-04-29 21:37:50.000000 flatpack-3.4.1/flatpack/main.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-01 14:27:37.907779 flatpack-3.4.1/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.1/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.1/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.1/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6876 2024-04-27 20:15:24.000000 flatpack-3.4.1/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.1/flatpack/session_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.1/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6413 2024-04-27 15:03:11.000000 flatpack-3.4.1/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-01 14:27:37.908031 flatpack-3.4.1/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-01 14:27:37.000000 flatpack-3.4.1/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      645 2024-05-01 14:27:37.000000 flatpack-3.4.1/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-01 14:27:37.000000 flatpack-3.4.1/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-01 14:27:37.000000 flatpack-3.4.1/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-01 14:27:37.000000 flatpack-3.4.1/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-01 14:27:37.000000 flatpack-3.4.1/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-01 14:27:37.908492 flatpack-3.4.1/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1089 2024-05-01 14:20:49.000000 flatpack-3.4.1/setup.py
```

### Comparing `flatpack-3.4.0/LICENSE` & `flatpack-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.0/PKG-INFO` & `flatpack-3.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.0
+Version: 3.4.1
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
@@ -15,14 +15,15 @@
 Requires-Dist: httpx==0.27.0
 Requires-Dist: huggingface-hub==0.22.2
 Requires-Dist: llama-cpp-python==0.2.65
 Requires-Dist: ngrok==1.2.0
 Requires-Dist: nltk==3.8.1
 Requires-Dist: olefile==0.47
 Requires-Dist: psutil==5.9.5
+Requires-Dist: pydantic==2.7.1
 Requires-Dist: pypdf==4.2.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: sentence-transformers==2.7.0
 Requires-Dist: toml==0.10.2
 Requires-Dist: uvicorn==0.29.0
 
 # Flatpack
@@ -113,14 +114,17 @@
 
 - **[olefile](https://pypi.org/project/olefile/)**\
   BSD License (BSD) ([LICENSE](https://github.com/decalage2/olefile/blob/master/LICENSE.txt))
 
 - **[psutil](https://pypi.org/project/psutil/)**\
   BSD License (BSD-3-Clause) ([LICENSE](https://github.com/giampaolo/psutil/blob/master/LICENSE))
 
+- **[pydantic](https://pypi.org/project/pydantic/)**\
+  MIT License ([LICENSE](https://github.com/pydantic/pydantic/blob/main/LICENSE))
+
 - **[pypdf](https://pypi.org/project/pypdf/)**\
   BSD License ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE))
 
 - **[requests](https://pypi.org/project/requests/)**\
   Apache Software License (Apache 2.0) ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
 
 - **[sentence-transformers](https://pypi.org/project/sentence-transformers/)**\
```

### Comparing `flatpack-3.4.0/README.md` & `flatpack-3.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,17 @@
 
 - **[olefile](https://pypi.org/project/olefile/)**\
   BSD License (BSD) ([LICENSE](https://github.com/decalage2/olefile/blob/master/LICENSE.txt))
 
 - **[psutil](https://pypi.org/project/psutil/)**\
   BSD License (BSD-3-Clause) ([LICENSE](https://github.com/giampaolo/psutil/blob/master/LICENSE))
 
+- **[pydantic](https://pypi.org/project/pydantic/)**\
+  MIT License ([LICENSE](https://github.com/pydantic/pydantic/blob/main/LICENSE))
+
 - **[pypdf](https://pypi.org/project/pypdf/)**\
   BSD License ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE))
 
 - **[requests](https://pypi.org/project/requests/)**\
   Apache Software License (Apache 2.0) ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
 
 - **[sentence-transformers](https://pypi.org/project/sentence-transformers/)**\
```

### Comparing `flatpack-3.4.0/flatpack/agent_manager.py` & `flatpack-3.4.1/flatpack/agent_manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,24 +34,14 @@
 
                 for pid in list(self.processes.keys()):
                     if not psutil.pid_exists(int(pid)):
                         del self.processes[pid]
         else:
             self.processes = {}
 
-    def load_engine(self):
-        self.engine = LlamaCPPEngine(
-            repo_id="microsoft/Phi-3-mini-4k-instruct-gguf",
-            filename="*q4.gguf",
-            n_ctx=4096,
-            n_threads=8,
-            verbose=True
-        )
-        print("Engine loaded successfully.")
-
     def spawn_agent(self, script_path):
         free_port = find_free_port()
         env = os.environ.copy()
         env['AGENT_PORT'] = str(free_port)
 
         process = subprocess.Popen(["python", script_path], env=env, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         pid = process.pid
```

### Comparing `flatpack-3.4.0/flatpack/datasets.py` & `flatpack-3.4.1/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.0/flatpack/engines/engine_llama_cpp.py` & `flatpack-3.4.1/flatpack/engines/engine_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.0/flatpack/engines/fast_api_test.py` & `flatpack-3.4.1/flatpack/engines/fast_api_test.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.0/flatpack/instructions.py` & `flatpack-3.4.1/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.0/flatpack/main.py` & `flatpack-3.4.1/flatpack/main.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.0/flatpack/modules/lstm.py` & `flatpack-3.4.1/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.0/flatpack/modules/rnn.py` & `flatpack-3.4.1/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.0/flatpack/parsers.py` & `flatpack-3.4.1/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.0/flatpack/vector_manager.py` & `flatpack-3.4.1/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.0/flatpack.egg-info/PKG-INFO` & `flatpack-3.4.1/flatpack.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.0
+Version: 3.4.1
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
@@ -15,14 +15,15 @@
 Requires-Dist: httpx==0.27.0
 Requires-Dist: huggingface-hub==0.22.2
 Requires-Dist: llama-cpp-python==0.2.65
 Requires-Dist: ngrok==1.2.0
 Requires-Dist: nltk==3.8.1
 Requires-Dist: olefile==0.47
 Requires-Dist: psutil==5.9.5
+Requires-Dist: pydantic==2.7.1
 Requires-Dist: pypdf==4.2.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: sentence-transformers==2.7.0
 Requires-Dist: toml==0.10.2
 Requires-Dist: uvicorn==0.29.0
 
 # Flatpack
@@ -113,14 +114,17 @@
 
 - **[olefile](https://pypi.org/project/olefile/)**\
   BSD License (BSD) ([LICENSE](https://github.com/decalage2/olefile/blob/master/LICENSE.txt))
 
 - **[psutil](https://pypi.org/project/psutil/)**\
   BSD License (BSD-3-Clause) ([LICENSE](https://github.com/giampaolo/psutil/blob/master/LICENSE))
 
+- **[pydantic](https://pypi.org/project/pydantic/)**\
+  MIT License ([LICENSE](https://github.com/pydantic/pydantic/blob/main/LICENSE))
+
 - **[pypdf](https://pypi.org/project/pypdf/)**\
   BSD License ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE))
 
 - **[requests](https://pypi.org/project/requests/)**\
   Apache Software License (Apache 2.0) ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
 
 - **[sentence-transformers](https://pypi.org/project/sentence-transformers/)**\
```

### Comparing `flatpack-3.4.0/flatpack.egg-info/SOURCES.txt` & `flatpack-3.4.1/flatpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.0/setup.py` & `flatpack-3.4.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.4.0",
+    version="3.4.1",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.5",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.2",
@@ -17,14 +17,15 @@
         "httpx==0.27.0",
         "huggingface-hub==0.22.2",
         "llama-cpp-python==0.2.65",
         "ngrok==1.2.0",
         "nltk==3.8.1",
         "olefile==0.47",
         "psutil==5.9.5",
+        "pydantic==2.7.1",
         "pypdf==4.2.0",
         "requests==2.31.0",
         "sentence-transformers==2.7.0",
         "toml==0.10.2",
         "uvicorn==0.29.0"
     ],
     author="Romlin Group AB",
```

