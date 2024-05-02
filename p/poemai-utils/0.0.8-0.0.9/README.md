# Comparing `tmp/poemai-utils-0.0.8.tar.gz` & `tmp/poemai-utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poemai-utils-0.0.8.tar", last modified: Tue Nov  7 12:51:02 2023, max compression
+gzip compressed data, was "poemai-utils-0.0.9.tar", last modified: Tue Nov  7 13:10:33 2023, max compression
```

## Comparing `poemai-utils-0.0.8.tar` & `poemai-utils-0.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 12:51:02.523322 poemai-utils-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-11-07 12:51:02.523322 poemai-utils-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-11-07 12:51:02.523322 poemai-utils-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      674 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 12:51:02.519322 poemai-utils-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 12:51:02.519322 poemai-utils-0.0.8/src/poemai_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 12:51:02.523322 poemai-utils-0.0.8/src/poemai_utils/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18027 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/aws/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/aws/dynamodb_emulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/basic_types_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/configuration_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 12:51:02.523322 poemai-utils-0.0.8/src/poemai_utils/embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/embeddings/cross_similarity_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/embeddings/embedder_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/embeddings/embedding_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/embeddings/embedding_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/embeddings/openai_embedder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/embeddings/self_similarity_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/embeddings/sentence_transformer_embedder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/embeddings/sgpt_embedder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 12:51:02.523322 poemai-utils-0.0.8/src/poemai_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14987 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/openai/ask.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/openai/llm_answer_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/openai/llm_answer_cache_dao.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/openai/openai_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/operations_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/simple_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-07 12:50:54.000000 poemai-utils-0.0.8/src/poemai_utils/utils_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 12:51:02.523322 poemai-utils-0.0.8/src/poemai_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-11-07 12:51:02.000000 poemai-utils-0.0.8/src/poemai_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2023-11-07 12:51:02.000000 poemai-utils-0.0.8/src/poemai_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-07 12:51:02.000000 poemai-utils-0.0.8/src/poemai_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-07 12:51:02.000000 poemai-utils-0.0.8/src/poemai_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-11-07 12:51:02.000000 poemai-utils-0.0.8/src/poemai_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-07 12:51:02.000000 poemai-utils-0.0.8/src/poemai_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 13:10:33.511710 poemai-utils-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2023-11-07 13:10:33.511710 poemai-utils-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2023-11-07 13:10:33.511710 poemai-utils-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 13:10:33.499710 poemai-utils-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 13:10:33.503710 poemai-utils-0.0.9/src/poemai_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 13:10:33.507710 poemai-utils-0.0.9/src/poemai_utils/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18027 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/aws/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/aws/dynamodb_emulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/basic_types_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/configuration_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 13:10:33.507710 poemai-utils-0.0.9/src/poemai_utils/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/embeddings/cross_similarity_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/embeddings/embedder_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/embeddings/embedding_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/embeddings/embedding_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/embeddings/openai_embedder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/embeddings/self_similarity_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/embeddings/sentence_transformer_embedder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/embeddings/sgpt_embedder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 13:10:33.511710 poemai-utils-0.0.9/src/poemai_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14987 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/openai/ask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/openai/llm_answer_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/openai/llm_answer_cache_dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/openai/openai_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/operations_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/simple_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-07 13:10:19.000000 poemai-utils-0.0.9/src/poemai_utils/utils_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 13:10:33.503710 poemai-utils-0.0.9/src/poemai_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2023-11-07 13:10:33.000000 poemai-utils-0.0.9/src/poemai_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2023-11-07 13:10:33.000000 poemai-utils-0.0.9/src/poemai_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-07 13:10:33.000000 poemai-utils-0.0.9/src/poemai_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-07 13:10:33.000000 poemai-utils-0.0.9/src/poemai_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2023-11-07 13:10:33.000000 poemai-utils-0.0.9/src/poemai_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-07 13:10:33.000000 poemai-utils-0.0.9/src/poemai_utils.egg-info/top_level.txt
```

### Comparing `poemai-utils-0.0.8/LICENSE.txt` & `poemai-utils-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/PKG-INFO` & `poemai-utils-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poemai-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Markus Emmenegger
 Author-email: markus.emmenegger@poemai.ch
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: sqlitedict
 Requires-Dist: httpx
 Requires-Dist: numpy
+Requires-Dist: openai<1.0.0
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: transformers; extra == "testing"
 
 # poemai-utils
```

### Comparing `poemai-utils-0.0.8/setup.cfg` & `poemai-utils-0.0.9/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	sqlitedict
 	httpx
 	numpy
+	openai<1.0.0
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `poemai-utils-0.0.8/setup.py` & `poemai-utils-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     PyScaffold helps you to put up the scaffold of your new Python project.
     Learn more under: https://pyscaffold.org/
 """
 from setuptools import setup
 
 if __name__ == "__main__":
     try:
-        setup(version="0.0.8")
+        setup(version="0.0.9")
     except:  # noqa
         print(
             "\n\nAn error occurred while building the project, "
             "please ensure you have the most updated version of setuptools, "
             "setuptools_scm and wheel with:\n"
             "   pip install -U setuptools setuptools_scm wheel\n\n"
         )
```

### Comparing `poemai-utils-0.0.8/src/poemai_utils/__init__.py` & `poemai-utils-0.0.9/src/poemai_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/src/poemai_utils/aws/dynamodb.py` & `poemai-utils-0.0.9/src/poemai_utils/aws/dynamodb.py`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/src/poemai_utils/aws/dynamodb_emulator.py` & `poemai-utils-0.0.9/src/poemai_utils/aws/dynamodb_emulator.py`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/src/poemai_utils/basic_types_utils.py` & `poemai-utils-0.0.9/src/poemai_utils/basic_types_utils.py`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/src/poemai_utils/embeddings/cross_similarity_analyzer.py` & `poemai-utils-0.0.9/src/poemai_utils/embeddings/cross_similarity_analyzer.py`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/src/poemai_utils/embeddings/embedding_cache.py` & `poemai-utils-0.0.9/src/poemai_utils/embeddings/embedding_cache.py`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/src/poemai_utils/embeddings/embedding_store.py` & `poemai-utils-0.0.9/src/poemai_utils/embeddings/embedding_store.py`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/src/poemai_utils/embeddings/openai_embedder.py` & `poemai-utils-0.0.9/src/poemai_utils/embeddings/openai_embedder.py`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/src/poemai_utils/embeddings/self_similarity_analyzer.py` & `poemai-utils-0.0.9/src/poemai_utils/embeddings/self_similarity_analyzer.py`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/src/poemai_utils/embeddings/sentence_transformer_embedder.py` & `poemai-utils-0.0.9/src/poemai_utils/embeddings/sentence_transformer_embedder.py`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/src/poemai_utils/embeddings/sgpt_embedder.py` & `poemai-utils-0.0.9/src/poemai_utils/embeddings/sgpt_embedder.py`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/src/poemai_utils/enum_utils.py` & `poemai-utils-0.0.9/src/poemai_utils/enum_utils.py`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/src/poemai_utils/file_utils.py` & `poemai-utils-0.0.9/src/poemai_utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/src/poemai_utils/openai/ask.py` & `poemai-utils-0.0.9/src/poemai_utils/openai/ask.py`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/src/poemai_utils/openai/llm_answer_cache.py` & `poemai-utils-0.0.9/src/poemai_utils/openai/llm_answer_cache.py`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/src/poemai_utils/openai/llm_answer_cache_dao.py` & `poemai-utils-0.0.9/src/poemai_utils/openai/llm_answer_cache_dao.py`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/src/poemai_utils/openai/openai_model.py` & `poemai-utils-0.0.9/src/poemai_utils/openai/openai_model.py`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/src/poemai_utils/simple_cache.py` & `poemai-utils-0.0.9/src/poemai_utils/simple_cache.py`

 * *Files identical despite different names*

### Comparing `poemai-utils-0.0.8/src/poemai_utils.egg-info/PKG-INFO` & `poemai-utils-0.0.9/src/poemai_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poemai-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Markus Emmenegger
 Author-email: markus.emmenegger@poemai.ch
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: sqlitedict
 Requires-Dist: httpx
 Requires-Dist: numpy
+Requires-Dist: openai<1.0.0
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: transformers; extra == "testing"
 
 # poemai-utils
```

### Comparing `poemai-utils-0.0.8/src/poemai_utils.egg-info/SOURCES.txt` & `poemai-utils-0.0.9/src/poemai_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

