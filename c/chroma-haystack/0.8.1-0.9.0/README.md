# Comparing `tmp/chroma_haystack-0.8.1.tar.gz` & `tmp/chroma_haystack-0.9.0.tar.gz`

## Comparing `chroma_haystack-0.8.1.tar` & `chroma_haystack-0.9.0.tar`

### file list

```diff
@@ -1,51 +1,50 @@
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/example.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_01.txt
--rw-r--r--   0        0        0    24228 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_02.txt
--rw-r--r--   0        0        0    23872 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_03.txt
--rw-r--r--   0        0        0    19131 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_04.txt
--rw-r--r--   0        0        0    27022 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_05.txt
--rw-r--r--   0        0        0    10639 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_06.txt
--rw-r--r--   0        0        0    15995 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_07.txt
--rw-r--r--   0        0        0    19379 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_08.txt
--rw-r--r--   0        0        0    11502 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_09.txt
--rw-r--r--   0        0        0    29200 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_10.txt
--rw-r--r--   0        0        0    13025 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_11.txt
--rw-r--r--   0        0        0    13433 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_12.txt
--rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_20.txt
--rw-r--r--   0        0        0    18456 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_21.txt
--rw-r--r--   0        0        0    14904 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_22.txt
--rw-r--r--   0        0        0    12744 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_23.txt
--rw-r--r--   0        0        0    20827 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_24.txt
--rw-r--r--   0        0        0    19176 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_25.txt
--rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_26.txt
--rw-r--r--   0        0        0    17709 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_27.txt
--rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_28.txt
--rw-r--r--   0        0        0    20259 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_29.txt
--rw-r--r--   0        0        0    22658 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_30.txt
--rw-r--r--   0        0        0    10399 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_31.txt
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_32.txt
--rw-r--r--   0        0        0    23554 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_40.txt
--rw-r--r--   0        0        0    64810 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_41.txt
--rw-r--r--   0        0        0    13853 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_42.txt
--rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_43.txt
--rw-r--r--   0        0        0    28948 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_44.txt
--rw-r--r--   0        0        0    17680 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_45.txt
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_46.txt
--rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_50.txt
--rw-r--r--   0        0        0    25503 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_51.txt
--rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_52.txt
--rw-r--r--   0        0        0    16836 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/example/data/usr_90.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/src/chroma_haystack/__about__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/src/chroma_haystack/__init__.py
--rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/src/chroma_haystack/document_store.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/src/chroma_haystack/errors.py
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/src/chroma_haystack/retriever.py
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/src/chroma_haystack/utils.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/tests/__init__.py
--rw-r--r--   0        0        0    10467 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/tests/test_document_store.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/tests/test_retriever.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/.gitignore
--rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/LICENSE
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/README.md
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 chroma_haystack-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/example.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_01.txt
+-rw-r--r--   0        0        0    24228 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_02.txt
+-rw-r--r--   0        0        0    23872 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_03.txt
+-rw-r--r--   0        0        0    19131 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_04.txt
+-rw-r--r--   0        0        0    27022 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_05.txt
+-rw-r--r--   0        0        0    10639 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_06.txt
+-rw-r--r--   0        0        0    15995 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_07.txt
+-rw-r--r--   0        0        0    19379 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_08.txt
+-rw-r--r--   0        0        0    11502 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_09.txt
+-rw-r--r--   0        0        0    29200 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_10.txt
+-rw-r--r--   0        0        0    13025 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_11.txt
+-rw-r--r--   0        0        0    13433 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_12.txt
+-rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_20.txt
+-rw-r--r--   0        0        0    18456 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_21.txt
+-rw-r--r--   0        0        0    14904 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_22.txt
+-rw-r--r--   0        0        0    12744 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_23.txt
+-rw-r--r--   0        0        0    20827 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_24.txt
+-rw-r--r--   0        0        0    19176 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_25.txt
+-rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_26.txt
+-rw-r--r--   0        0        0    17709 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_27.txt
+-rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_28.txt
+-rw-r--r--   0        0        0    20259 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_29.txt
+-rw-r--r--   0        0        0    22658 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_30.txt
+-rw-r--r--   0        0        0    10399 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_31.txt
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_32.txt
+-rw-r--r--   0        0        0    23554 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_40.txt
+-rw-r--r--   0        0        0    64810 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_41.txt
+-rw-r--r--   0        0        0    13853 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_42.txt
+-rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_43.txt
+-rw-r--r--   0        0        0    28948 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_44.txt
+-rw-r--r--   0        0        0    17680 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_45.txt
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_46.txt
+-rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_50.txt
+-rw-r--r--   0        0        0    25503 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_51.txt
+-rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_52.txt
+-rw-r--r--   0        0        0    16836 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/example/data/usr_90.txt
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/src/chroma_haystack/__init__.py
+-rw-r--r--   0        0        0    12232 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/src/chroma_haystack/document_store.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/src/chroma_haystack/errors.py
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/src/chroma_haystack/retriever.py
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/src/chroma_haystack/utils.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0    10467 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/tests/test_document_store.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/tests/test_retriever.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/.gitignore
+-rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/README.md
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 chroma_haystack-0.9.0/PKG-INFO
```

### Comparing `chroma_haystack-0.8.1/example/example.py` & `chroma_haystack-0.9.0/example/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Colab: https://colab.research.google.com/drive/1YpDetI8BRbObPDEVdfqUcwhEX9UUXP-m?usp=sharing
 import os
 from pathlib import Path
 
 from haystack import Pipeline
-from haystack.components.file_converters import TextFileToDocument
+from haystack.components.converters import TextFileToDocument
 from haystack.components.writers import DocumentWriter
 
 from chroma_haystack import ChromaDocumentStore
 from chroma_haystack.retriever import ChromaQueryRetriever
 
 HERE = Path(__file__).resolve().parent
 file_paths = [HERE / "data" / Path(name) for name in os.listdir("data")]
@@ -15,15 +15,15 @@
 # Chroma is used in-memory so we use the same instances in the two pipelines below
 document_store = ChromaDocumentStore()
 
 indexing = Pipeline()
 indexing.add_component("converter", TextFileToDocument())
 indexing.add_component("writer", DocumentWriter(document_store))
 indexing.connect("converter", "writer")
-indexing.run({"converter": {"paths": file_paths}})
+indexing.run({"converter": {"sources": file_paths}})
 
 querying = Pipeline()
 querying.add_component("retriever", ChromaQueryRetriever(document_store))
 results = querying.run({"retriever": {"queries": ["Variable declarations"], "top_k": 3}})
 
-for d in results["retriever"][0]:
-    print(d.metadata, d.score)
+for d in results["retriever"]["documents"][0]:
+    print(d.meta, d.score)
```

### Comparing `chroma_haystack-0.8.1/example/data/usr_01.txt` & `chroma_haystack-0.9.0/example/data/usr_01.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_02.txt` & `chroma_haystack-0.9.0/example/data/usr_02.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_03.txt` & `chroma_haystack-0.9.0/example/data/usr_03.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_04.txt` & `chroma_haystack-0.9.0/example/data/usr_04.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_05.txt` & `chroma_haystack-0.9.0/example/data/usr_05.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_06.txt` & `chroma_haystack-0.9.0/example/data/usr_06.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_07.txt` & `chroma_haystack-0.9.0/example/data/usr_07.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_08.txt` & `chroma_haystack-0.9.0/example/data/usr_08.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_09.txt` & `chroma_haystack-0.9.0/example/data/usr_09.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_10.txt` & `chroma_haystack-0.9.0/example/data/usr_10.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_11.txt` & `chroma_haystack-0.9.0/example/data/usr_11.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_12.txt` & `chroma_haystack-0.9.0/example/data/usr_12.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_20.txt` & `chroma_haystack-0.9.0/example/data/usr_20.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_21.txt` & `chroma_haystack-0.9.0/example/data/usr_21.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_22.txt` & `chroma_haystack-0.9.0/example/data/usr_22.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_23.txt` & `chroma_haystack-0.9.0/example/data/usr_23.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_24.txt` & `chroma_haystack-0.9.0/example/data/usr_24.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_25.txt` & `chroma_haystack-0.9.0/example/data/usr_25.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_26.txt` & `chroma_haystack-0.9.0/example/data/usr_26.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_27.txt` & `chroma_haystack-0.9.0/example/data/usr_27.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_28.txt` & `chroma_haystack-0.9.0/example/data/usr_28.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_29.txt` & `chroma_haystack-0.9.0/example/data/usr_29.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_30.txt` & `chroma_haystack-0.9.0/example/data/usr_30.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_31.txt` & `chroma_haystack-0.9.0/example/data/usr_31.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_32.txt` & `chroma_haystack-0.9.0/example/data/usr_32.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_40.txt` & `chroma_haystack-0.9.0/example/data/usr_40.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_41.txt` & `chroma_haystack-0.9.0/example/data/usr_41.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_42.txt` & `chroma_haystack-0.9.0/example/data/usr_42.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_43.txt` & `chroma_haystack-0.9.0/example/data/usr_43.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_44.txt` & `chroma_haystack-0.9.0/example/data/usr_44.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_45.txt` & `chroma_haystack-0.9.0/example/data/usr_45.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_46.txt` & `chroma_haystack-0.9.0/example/data/usr_46.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_50.txt` & `chroma_haystack-0.9.0/example/data/usr_50.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_51.txt` & `chroma_haystack-0.9.0/example/data/usr_51.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_52.txt` & `chroma_haystack-0.9.0/example/data/usr_52.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/example/data/usr_90.txt` & `chroma_haystack-0.9.0/example/data/usr_90.txt`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/src/chroma_haystack/document_store.py` & `chroma_haystack-0.9.0/src/chroma_haystack/document_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -243,18 +243,14 @@
                 if len(value) == 1:
                     where[field] = value[0]
                     continue
 
                 # if the list contains multiple items, we need an $or chain
                 for v in value:
                     where["$or"].append({field: v})
-            elif field == "mime_type":
-                # Schedule for removal the original key, we're going to change it
-                keys_to_remove.append(field)
-                where["_mime_type"] = value
 
         for k in keys_to_remove:
             del filters[k]
 
         final_where = dict(filters | where)
         try:
             if final_where:
@@ -306,16 +302,15 @@
                 document_dict: Dict[str, Any] = {
                     "id": result["ids"][i][j],
                     "content": documents[i][j],
                 }
 
                 # prepare metadata
                 if metadatas := result.get("metadatas"):
-                    document_dict["metadata"] = dict(metadatas[i][j])
-                    document_dict["mime_type"] = document_dict["metadata"].pop("_mime_type")
+                    document_dict["meta"] = dict(metadatas[i][j])
 
                 if embeddings := result.get("embeddings"):
                     document_dict["embedding"] = np.array(embeddings[i][j])
 
                 if distances := result.get("distances"):
                     document_dict["score"] = distances[i][j]
```

### Comparing `chroma_haystack-0.8.1/src/chroma_haystack/retriever.py` & `chroma_haystack-0.9.0/src/chroma_haystack/retriever.py`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/src/chroma_haystack/utils.py` & `chroma_haystack-0.9.0/src/chroma_haystack/utils.py`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/tests/test_document_store.py` & `chroma_haystack-0.9.0/tests/test_document_store.py`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/tests/test_retriever.py` & `chroma_haystack-0.9.0/tests/test_retriever.py`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/.gitignore` & `chroma_haystack-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/LICENSE` & `chroma_haystack-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/README.md` & `chroma_haystack-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `chroma_haystack-0.8.1/pyproject.toml` & `chroma_haystack-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -20,24 +20,29 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "haystack-ai",
-  "chromadb",
+  "chromadb<0.4.20",  #  FIXME: investigate why filtering tests broke on 0.4.20
 ]
 
 [project.urls]
-Documentation = "https://github.com/masci/chroma-haystack#readme"
-Issues = "https://github.com/masci/chroma-haystack/issues"
-Source = "https://github.com/masci/chroma-haystack"
+Documentation = "https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/chroma#readme"
+Issues = "https://github.com/deepset-ai/haystack-core-integrations/issues"
+Source = "https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/chroma"
 
 [tool.hatch.version]
-path = "src/chroma_haystack/__about__.py"
+source = "vcs"
+tag-pattern = 'integrations\/chroma-v(?P<version>.*)'
+
+[tool.hatch.version.raw-options]
+root = "../.."
+git_describe_command = 'git describe --tags --match="integrations/chroma-v[0-9]*"'
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
 ]
 [tool.hatch.envs.default.scripts]
```

### Comparing `chroma_haystack-0.8.1/PKG-INFO` & `chroma_haystack-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: chroma-haystack
-Version: 0.8.1
-Project-URL: Documentation, https://github.com/masci/chroma-haystack#readme
-Project-URL: Issues, https://github.com/masci/chroma-haystack/issues
-Project-URL: Source, https://github.com/masci/chroma-haystack
+Version: 0.9.0
+Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/chroma#readme
+Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
+Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/chroma
 Author-email: John Doe <jd@example.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
-Requires-Dist: chromadb
+Requires-Dist: chromadb<0.4.20
 Requires-Dist: haystack-ai
 Description-Content-Type: text/markdown
 
 # Chroma Document Store for Haystack
 
 [![PyPI - Version](https://img.shields.io/pypi/v/chroma-haystack.svg)](https://pypi.org/project/chroma-haystack)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/chroma-haystack.svg)](https://pypi.org/project/chroma-haystack)
```

