# Comparing `tmp/flatpack-3.4.5.tar.gz` & `tmp/flatpack-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.4.5.tar", last modified: Thu May  2 09:48:20 2024, max compression
+gzip compressed data, was "flatpack-3.4.6.tar", last modified: Thu May  2 10:07:00 2024, max compression
```

## Comparing `flatpack-3.4.5.tar` & `flatpack-3.4.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 09:48:20.121767 flatpack-3.4.5/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.5/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 09:48:20.121575 flatpack-3.4.5/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-01 14:25:58.000000 flatpack-3.4.5/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 09:48:20.119223 flatpack-3.4.5/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      111 2024-04-27 22:37:06.000000 flatpack-3.4.5/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.5/flatpack/agent_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.5/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.5/flatpack/datasets.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 09:48:20.120509 flatpack-3.4.5/flatpack/engines/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.5/flatpack/engines/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      796 2024-05-02 08:44:24.000000 flatpack-3.4.5/flatpack/engines/engine_llama_cpp.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      922 2024-05-02 08:44:56.000000 flatpack-3.4.5/flatpack/engines/fast_api_test.py
--rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.5/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.5/flatpack/load_modules.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    26214 2024-04-29 21:37:50.000000 flatpack-3.4.5/flatpack/main.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 09:48:20.121081 flatpack-3.4.5/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.5/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.5/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.5/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6876 2024-04-27 20:15:24.000000 flatpack-3.4.5/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.5/flatpack/session_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.5/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6413 2024-04-27 15:03:11.000000 flatpack-3.4.5/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 09:48:20.121334 flatpack-3.4.5/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 09:48:20.000000 flatpack-3.4.5/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      645 2024-05-02 09:48:20.000000 flatpack-3.4.5/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-02 09:48:20.000000 flatpack-3.4.5/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-02 09:48:20.000000 flatpack-3.4.5/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-02 09:48:20.000000 flatpack-3.4.5/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-02 09:48:20.000000 flatpack-3.4.5/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-02 09:48:20.121810 flatpack-3.4.5/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)     1089 2024-05-02 08:45:20.000000 flatpack-3.4.5/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 10:07:00.811749 flatpack-3.4.6/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.6/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 10:07:00.811564 flatpack-3.4.6/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-01 14:25:58.000000 flatpack-3.4.6/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 10:07:00.808968 flatpack-3.4.6/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      111 2024-04-27 22:37:06.000000 flatpack-3.4.6/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.6/flatpack/agent_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.6/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.6/flatpack/datasets.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 10:07:00.810405 flatpack-3.4.6/flatpack/engines/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.6/flatpack/engines/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      796 2024-05-02 08:44:24.000000 flatpack-3.4.6/flatpack/engines/engine_llama_cpp.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      922 2024-05-02 08:44:56.000000 flatpack-3.4.6/flatpack/engines/fast_api_test.py
+-rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.6/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.6/flatpack/load_modules.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    26234 2024-05-02 10:00:01.000000 flatpack-3.4.6/flatpack/main.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 10:07:00.811087 flatpack-3.4.6/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.6/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.6/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.6/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6876 2024-04-27 20:15:24.000000 flatpack-3.4.6/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.6/flatpack/session_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.6/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6413 2024-04-27 15:03:11.000000 flatpack-3.4.6/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 10:07:00.811333 flatpack-3.4.6/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 10:07:00.000000 flatpack-3.4.6/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      645 2024-05-02 10:07:00.000000 flatpack-3.4.6/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-02 10:07:00.000000 flatpack-3.4.6/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-02 10:07:00.000000 flatpack-3.4.6/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-02 10:07:00.000000 flatpack-3.4.6/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-02 10:07:00.000000 flatpack-3.4.6/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-02 10:07:00.811790 flatpack-3.4.6/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1089 2024-05-02 09:57:31.000000 flatpack-3.4.6/setup.py
```

### Comparing `flatpack-3.4.5/LICENSE` & `flatpack-3.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.5/PKG-INFO` & `flatpack-3.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.5
+Version: 3.4.6
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.4.5/README.md` & `flatpack-3.4.6/README.md`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.5/flatpack/agent_manager.py` & `flatpack-3.4.6/flatpack/agent_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.5/flatpack/datasets.py` & `flatpack-3.4.6/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.5/flatpack/engines/engine_llama_cpp.py` & `flatpack-3.4.6/flatpack/engines/engine_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.5/flatpack/engines/fast_api_test.py` & `flatpack-3.4.6/flatpack/engines/fast_api_test.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.5/flatpack/instructions.py` & `flatpack-3.4.6/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.5/flatpack/main.py` & `flatpack-3.4.6/flatpack/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -529,15 +529,15 @@
     return parser
 
 
 def fpk_cli_handle_add_pdf(pdf_path, vm):
     if not os.path.exists(pdf_path):
         print(f"❌ PDF file does not exist: '{pdf_path}'.")
         return
-    vm.add_pdf(pdf_path)
+    vm.add_pdf(pdf_path, pdf_path)
     print(f"✅ Added text from PDF: '{pdf_path}' to the vector database.")
 
 
 def fpk_cli_handle_add_url(url, vm):
     try:
         response = requests.head(url, allow_redirects=True, timeout=5)
         if response.status_code >= 200 and response.status_code < 400:
@@ -662,15 +662,15 @@
 
 def fpk_cli_handle_vector_commands(args, session):
     print("Handling vector commands...")
 
     vm = VectorManager(model_name='all-MiniLM-L6-v2', directory=getattr(args, 'data_dir', '.'))
 
     if args.vector_command == 'add-texts':
-        vm.add_texts(args.texts)
+        vm.add_texts(args.texts, "manual")
         print(f"Added {len(args.texts)} texts to the database.")
     elif args.vector_command == 'search-text':
         results = vm.search_vectors(args.query)
         if results:
             print("Search results:")
             for result in results:
                 print(f"{result['id']}: {result['text']}\n")
```

### Comparing `flatpack-3.4.5/flatpack/modules/lstm.py` & `flatpack-3.4.6/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.5/flatpack/modules/rnn.py` & `flatpack-3.4.6/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.5/flatpack/parsers.py` & `flatpack-3.4.6/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.5/flatpack/vector_manager.py` & `flatpack-3.4.6/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.5/flatpack.egg-info/PKG-INFO` & `flatpack-3.4.6/flatpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.5
+Version: 3.4.6
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.4.5/flatpack.egg-info/SOURCES.txt` & `flatpack-3.4.6/flatpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.5/setup.py` & `flatpack-3.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.4.5",
+    version="3.4.6",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.5",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.2",
```

