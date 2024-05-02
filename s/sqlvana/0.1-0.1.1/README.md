# Comparing `tmp/sqlvana-0.1.tar.gz` & `tmp/sqlvana-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlvana-0.1.tar", last modified: Tue Apr 30 12:58:27 2024, max compression
+gzip compressed data, was "sqlvana-0.1.1.tar", last modified: Wed May  1 09:33:42 2024, max compression
```

## Comparing `sqlvana-0.1.tar` & `sqlvana-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,67 @@
-drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-04-30 12:58:27.332605 sqlvana-0.1/
--rw-r--r--   0 lidi10     (501) staff       (20)     1069 2024-04-30 12:04:48.000000 sqlvana-0.1/LICENSE
--rw-r--r--   0 lidi10     (501) staff       (20)      456 2024-04-30 12:58:27.332398 sqlvana-0.1/PKG-INFO
--rw-r--r--   0 lidi10     (501) staff       (20)       41 2024-04-30 12:04:07.000000 sqlvana-0.1/README.md
--rw-r--r--   0 lidi10     (501) staff       (20)       38 2024-04-30 12:58:27.332648 sqlvana-0.1/setup.cfg
--rw-r--r--   0 lidi10     (501) staff       (20)      482 2024-04-30 12:58:23.000000 sqlvana-0.1/setup.py
-drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-04-30 12:58:27.331675 sqlvana-0.1/sqlvana.egg-info/
--rw-r--r--   0 lidi10     (501) staff       (20)      456 2024-04-30 12:58:27.000000 sqlvana-0.1/sqlvana.egg-info/PKG-INFO
--rw-r--r--   0 lidi10     (501) staff       (20)      224 2024-04-30 12:58:27.000000 sqlvana-0.1/sqlvana.egg-info/SOURCES.txt
--rw-r--r--   0 lidi10     (501) staff       (20)        1 2024-04-30 12:58:27.000000 sqlvana-0.1/sqlvana.egg-info/dependency_links.txt
--rw-r--r--   0 lidi10     (501) staff       (20)       66 2024-04-30 12:58:27.000000 sqlvana-0.1/sqlvana.egg-info/requires.txt
--rw-r--r--   0 lidi10     (501) staff       (20)        1 2024-04-30 12:58:27.000000 sqlvana-0.1/sqlvana.egg-info/top_level.txt
-drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-04-30 12:58:27.332017 sqlvana-0.1/tests/
--rw-r--r--   0 lidi10     (501) staff       (20)     1231 2024-04-30 12:03:41.000000 sqlvana-0.1/tests/test_imports.py
--rw-r--r--   0 lidi10     (501) staff       (20)     7768 2024-04-30 12:03:41.000000 sqlvana-0.1/tests/test_sqlvana.py
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.641620 sqlvana-0.1.1/
+-rw-r--r--   0 lidi10     (501) staff       (20)     1069 2024-04-30 12:04:48.000000 sqlvana-0.1.1/LICENSE
+-rw-r--r--   0 lidi10     (501) staff       (20)      458 2024-05-01 09:33:42.641347 sqlvana-0.1.1/PKG-INFO
+-rw-r--r--   0 lidi10     (501) staff       (20)       41 2024-04-30 12:04:07.000000 sqlvana-0.1.1/README.md
+-rw-r--r--   0 lidi10     (501) staff       (20)       38 2024-05-01 09:33:42.641669 sqlvana-0.1.1/setup.cfg
+-rw-r--r--   0 lidi10     (501) staff       (20)      591 2024-05-01 09:33:41.000000 sqlvana-0.1.1/setup.py
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.613387 sqlvana-0.1.1/src/
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.616181 sqlvana-0.1.1/src/sqlvana/
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.617988 sqlvana-0.1.1/src/sqlvana/ZhipuAI/
+-rw-r--r--   0 lidi10     (501) staff       (20)     8725 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/ZhipuAI/ZhipuAI_Chat.py
+-rw-r--r--   0 lidi10     (501) staff       (20)     2849 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/ZhipuAI/ZhipuAI_embeddings.py
+-rw-r--r--   0 lidi10     (501) staff       (20)      116 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/ZhipuAI/__init__.py
+-rw-r--r--   0 lidi10     (501) staff       (20)     9248 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/__init__.py
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.619075 sqlvana-0.1.1/src/sqlvana/anthropic/
+-rw-r--r--   0 lidi10     (501) staff       (20)       43 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/anthropic/__init__.py
+-rw-r--r--   0 lidi10     (501) staff       (20)     2615 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/anthropic/anthropic_chat.py
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.621626 sqlvana-0.1.1/src/sqlvana/base/
+-rw-r--r--   0 lidi10     (501) staff       (20)       28 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/base/__init__.py
+-rw-r--r--   0 lidi10     (501) staff       (20)    58145 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/base/base.py
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.624644 sqlvana-0.1.1/src/sqlvana/chromadb/
+-rw-r--r--   0 lidi10     (501) staff       (20)       50 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/chromadb/__init__.py
+-rw-r--r--   0 lidi10     (501) staff       (20)     8792 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/chromadb/chromadb_vector.py
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.625826 sqlvana-0.1.1/src/sqlvana/exceptions/
+-rw-r--r--   0 lidi10     (501) staff       (20)      685 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/exceptions/__init__.py
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.634900 sqlvana-0.1.1/src/sqlvana/flask/
+-rw-r--r--   0 lidi10     (501) staff       (20)    23859 2024-04-30 13:42:55.000000 sqlvana-0.1.1/src/sqlvana/flask/__init__.py
+-rw-r--r--   0 lidi10     (501) staff       (20)   184082 2024-04-30 13:41:39.000000 sqlvana-0.1.1/src/sqlvana/flask/assets.py
+-rw-r--r--   0 lidi10     (501) staff       (20)     1246 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/flask/auth.py
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.635532 sqlvana-0.1.1/src/sqlvana/google/
+-rw-r--r--   0 lidi10     (501) staff       (20)       41 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/google/__init__.py
+-rw-r--r--   0 lidi10     (501) staff       (20)     1584 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/google/gemini_chat.py
+-rw-r--r--   0 lidi10     (501) staff       (20)      313 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/local.py
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.636201 sqlvana-0.1.1/src/sqlvana/marqo/
+-rw-r--r--   0 lidi10     (501) staff       (20)       37 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/marqo/__init__.py
+-rw-r--r--   0 lidi10     (501) staff       (20)     5242 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/marqo/marqo.py
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.636696 sqlvana-0.1.1/src/sqlvana/mistral/
+-rw-r--r--   0 lidi10     (501) staff       (20)       29 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/mistral/__init__.py
+-rw-r--r--   0 lidi10     (501) staff       (20)     1508 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/mistral/mistral.py
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.637097 sqlvana-0.1.1/src/sqlvana/ollama/
+-rw-r--r--   0 lidi10     (501) staff       (20)       27 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/ollama/__init__.py
+-rw-r--r--   0 lidi10     (501) staff       (20)     2418 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/ollama/ollama.py
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.637796 sqlvana-0.1.1/src/sqlvana/openai/
+-rw-r--r--   0 lidi10     (501) staff       (20)       86 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/openai/__init__.py
+-rw-r--r--   0 lidi10     (501) staff       (20)     4764 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/openai/openai_chat.py
+-rw-r--r--   0 lidi10     (501) staff       (20)     1260 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/openai/openai_embeddings.py
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.638253 sqlvana-0.1.1/src/sqlvana/qdrant/
+-rw-r--r--   0 lidi10     (501) staff       (20)       73 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/qdrant/__init__.py
+-rw-r--r--   0 lidi10     (501) staff       (20)    11940 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/qdrant/qdrant.py
+-rw-r--r--   0 lidi10     (501) staff       (20)     1856 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/remote.py
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.639100 sqlvana-0.1.1/src/sqlvana/types/
+-rw-r--r--   0 lidi10     (501) staff       (20)     4957 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/types/__init__.py
+-rw-r--r--   0 lidi10     (501) staff       (20)     2247 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/utils.py
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.639784 sqlvana-0.1.1/src/sqlvana/vannadb/
+-rw-r--r--   0 lidi10     (501) staff       (20)       48 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/vannadb/__init__.py
+-rw-r--r--   0 lidi10     (501) staff       (20)     6168 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/vannadb/vannadb_vector.py
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.640612 sqlvana-0.1.1/src/sqlvana/vllm/
+-rw-r--r--   0 lidi10     (501) staff       (20)       23 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/vllm/__init__.py
+-rw-r--r--   0 lidi10     (501) staff       (20)     2427 2024-04-30 12:03:41.000000 sqlvana-0.1.1/src/sqlvana/vllm/vllm.py
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.617055 sqlvana-0.1.1/src/sqlvana.egg-info/
+-rw-r--r--   0 lidi10     (501) staff       (20)      458 2024-05-01 09:33:42.000000 sqlvana-0.1.1/src/sqlvana.egg-info/PKG-INFO
+-rw-r--r--   0 lidi10     (501) staff       (20)     1326 2024-05-01 09:33:42.000000 sqlvana-0.1.1/src/sqlvana.egg-info/SOURCES.txt
+-rw-r--r--   0 lidi10     (501) staff       (20)        1 2024-05-01 09:33:42.000000 sqlvana-0.1.1/src/sqlvana.egg-info/dependency_links.txt
+-rw-r--r--   0 lidi10     (501) staff       (20)       66 2024-05-01 09:33:42.000000 sqlvana-0.1.1/src/sqlvana.egg-info/requires.txt
+-rw-r--r--   0 lidi10     (501) staff       (20)        8 2024-05-01 09:33:42.000000 sqlvana-0.1.1/src/sqlvana.egg-info/top_level.txt
+drwxr-xr-x   0 lidi10     (501) staff       (20)        0 2024-05-01 09:33:42.640969 sqlvana-0.1.1/tests/
+-rw-r--r--   0 lidi10     (501) staff       (20)     1231 2024-04-30 12:03:41.000000 sqlvana-0.1.1/tests/test_imports.py
+-rw-r--r--   0 lidi10     (501) staff       (20)     7768 2024-05-01 09:06:19.000000 sqlvana-0.1.1/tests/test_sqlvana.py
```

### Comparing `sqlvana-0.1/LICENSE` & `sqlvana-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlvana-0.1/tests/test_imports.py` & `sqlvana-0.1.1/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `sqlvana-0.1/tests/test_sqlvana.py` & `sqlvana-0.1.1/tests/test_sqlvana.py`

 * *Files identical despite different names*

