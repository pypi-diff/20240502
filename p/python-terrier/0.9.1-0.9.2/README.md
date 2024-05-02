# Comparing `tmp/python-terrier-0.9.1.tar.gz` & `tmp/python-terrier-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-terrier-0.9.1.tar", last modified: Fri Nov 11 15:01:25 2022, max compression
+gzip compressed data, was "dist/python-terrier-0.9.2.tar", last modified: Mon Dec 19 12:23:17 2022, max compression
```

## Comparing `python-terrier-0.9.1.tar` & `python-terrier-0.9.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-11 15:01:25.000000 python-terrier-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (116)    16726 2022-11-11 15:01:22.000000 python-terrier-0.9.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)       66 2022-11-11 15:01:22.000000 python-terrier-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    11050 2022-11-11 15:01:25.000000 python-terrier-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     9262 2022-11-11 15:01:22.000000 python-terrier-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-11 15:01:25.000000 python-terrier-0.9.1/pyterrier/
--rw-r--r--   0 runner    (1001) docker     (116)    15431 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6884 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/anserini.py
--rw-r--r--   0 runner    (1001) docker     (116)     9015 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/apply.py
--rw-r--r--   0 runner    (1001) docker     (116)     7689 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/apply_base.py
--rw-r--r--   0 runner    (1001) docker     (116)    38045 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/batchretrieve.py
--rw-r--r--   0 runner    (1001) docker     (116)     9850 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (116)     6764 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/cache.py
--rw-r--r--   0 runner    (1001) docker     (116)    53269 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/datasets.py
--rw-r--r--   0 runner    (1001) docker     (116)     4204 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/debug.py
--rw-r--r--   0 runner    (1001) docker     (116)    48740 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/index.py
--rw-r--r--   0 runner    (1001) docker     (116)    15915 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/io.py
--rw-r--r--   0 runner    (1001) docker     (116)    11978 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/ltr.py
--rw-r--r--   0 runner    (1001) docker     (116)     2446 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/mavenresolver.py
--rw-r--r--   0 runner    (1001) docker     (116)      166 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/measures.py
--rw-r--r--   0 runner    (1001) docker     (116)     8965 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/model.py
--rw-r--r--   0 runner    (1001) docker     (116)     5024 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/new.py
--rw-r--r--   0 runner    (1001) docker     (116)    15382 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/ops.py
--rw-r--r--   0 runner    (1001) docker     (116)     4015 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/parallel.py
--rw-r--r--   0 runner    (1001) docker     (116)    40730 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (116)    24971 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/rewrite.py
--rw-r--r--   0 runner    (1001) docker     (116)    21360 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/text.py
--rw-r--r--   0 runner    (1001) docker     (116)    14508 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/transformer.py
--rw-r--r--   0 runner    (1001) docker     (116)     3985 2022-11-11 15:01:22.000000 python-terrier-0.9.1/pyterrier/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-11 15:01:25.000000 python-terrier-0.9.1/python_terrier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    11050 2022-11-11 15:01:25.000000 python-terrier-0.9.1/python_terrier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      749 2022-11-11 15:01:25.000000 python-terrier-0.9.1/python_terrier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-11 15:01:25.000000 python-terrier-0.9.1/python_terrier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      213 2022-11-11 15:01:25.000000 python-terrier-0.9.1/python_terrier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2022-11-11 15:01:25.000000 python-terrier-0.9.1/python_terrier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       46 2022-11-11 15:01:22.000000 python-terrier-0.9.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (116)      213 2022-11-11 15:01:22.000000 python-terrier-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-11-11 15:01:25.000000 python-terrier-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2402 2022-11-11 15:01:22.000000 python-terrier-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-19 12:23:17.000000 python-terrier-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (116)    16726 2022-12-19 12:23:16.000000 python-terrier-0.9.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       66 2022-12-19 12:23:16.000000 python-terrier-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    11683 2022-12-19 12:23:17.000000 python-terrier-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     9879 2022-12-19 12:23:16.000000 python-terrier-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-19 12:23:17.000000 python-terrier-0.9.2/pyterrier/
+-rw-r--r--   0 runner    (1001) docker     (116)    15431 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6884 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/anserini.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9501 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/apply.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9960 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/apply_base.py
+-rw-r--r--   0 runner    (1001) docker     (116)    38067 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/batchretrieve.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9850 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6764 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)    53269 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4204 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/debug.py
+-rw-r--r--   0 runner    (1001) docker     (116)    50867 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/index.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15915 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/io.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11978 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/ltr.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2446 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/mavenresolver.py
+-rw-r--r--   0 runner    (1001) docker     (116)      166 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/measures.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9130 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/model.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5024 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/new.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15545 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/ops.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4015 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (116)    40730 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (116)    24971 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/rewrite.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21492 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/text.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14508 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3985 2022-12-19 12:23:16.000000 python-terrier-0.9.2/pyterrier/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-19 12:23:17.000000 python-terrier-0.9.2/python_terrier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    11683 2022-12-19 12:23:17.000000 python-terrier-0.9.2/python_terrier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      749 2022-12-19 12:23:17.000000 python-terrier-0.9.2/python_terrier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-19 12:23:17.000000 python-terrier-0.9.2/python_terrier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      218 2022-12-19 12:23:17.000000 python-terrier-0.9.2/python_terrier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       10 2022-12-19 12:23:17.000000 python-terrier-0.9.2/python_terrier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2022-12-19 12:23:16.000000 python-terrier-0.9.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      218 2022-12-19 12:23:16.000000 python-terrier-0.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2022-12-19 12:23:17.000000 python-terrier-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2402 2022-12-19 12:23:16.000000 python-terrier-0.9.2/setup.py
```

### Comparing `python-terrier-0.9.1/LICENSE.txt` & `python-terrier-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-terrier-0.9.1/PKG-INFO` & `python-terrier-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-terrier
-Version: 0.9.1
+Version: 0.9.2
 Summary: Terrier IR platform Python API
 Home-page: https://github.com/terrier-org/pyterrier
 Author: Craig Macdonald
 Author-email: craigm@dcs.gla.ac.uk
 License: UNKNOWN
 Description: ![Python package](https://github.com/terrier-org/pyterrier/workflows/Python%20package/badge.svg) 
         [![PyPI version](https://badge.fury.io/py/python-terrier.svg)](https://badge.fury.io/py/python-terrier)
@@ -28,18 +28,18 @@
         1. You need to hava Java installed. Pyjnius/PyTerrier will pick up the location automatically.
         2. `pip install python-terrier`
         
         # Indexing
         
         PyTerrier has a number of useful classes for creating indices:
         
-         - You can create an index from TREC formatted collection using TRECCollectionIndexer.    
-         - For TXT, PDF, Microsoft Word files, etc files you can use FilesIndexer.
-         - For Pandas Dataframe you can use DFIndexer.
-         - For any abitrary iterable dictionaries, you can use IterDictIndexer.
+         - You can create an index from TREC formatted collection using [TRECCollectionIndexer](https://pyterrier.readthedocs.io/en/latest/terrier-indexing.html#treccollectionindexer).    
+         - For TXT, PDF, Microsoft Word files, etc files you can use [FilesIndexer](https://pyterrier.readthedocs.io/en/latest/terrier-indexing.html#filesindexer).
+         - For Pandas Dataframe you can use [DFIndexer](https://pyterrier.readthedocs.io/en/latest/terrier-indexing.html#dfindexer).
+         - For any abitrary iterable dictionaries, you can use [IterDictIndexer](https://pyterrier.readthedocs.io/en/latest/terrier-indexing.html#iterdictindexer).
         
         See the [indexing documentation](https://pyterrier.readthedocs.io/en/latest/terrier-indexing.html), or the examples in the [indexing notebook](examples/notebooks/indexing.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/terrier-org/pyterrier/blob/master/examples/notebooks/indexing.ipynb)
         
         # Retrieval and Evaluation
         
         ```python
         topics = pt.io.read_topics(topicsFile)
@@ -73,16 +73,18 @@
         # Neural Reranking and Dense Retrieval
         
         PyTerrier has additional plugins for BERT (through OpenNIR), T5, ColBERT, ANCE, DeepCT and doc2query.
         
          - OpenNIR: [[Github](https://github.com/Georgetown-IR-Lab/OpenNIR)] [[Documentation](https://opennir.net/)]
          - PyTerrier_ANCE: [[Github](https://github.com/terrierteam/pyterrier_ance)] - dense retrieval
          - PyTerrier_ColBERT: [[Github](https://github.com/terrierteam/pyterrier_colbert)] - dense retrieval and/or neural reranking
-         - PyTerrier_T5: [[Github](https://github.com/terrierteam/pyterrier_t5)] - neural reranking
+         - PyTerrier_PISA: [[Github](https://github.com/terrierteam/pyterrier_pisa)] - fast in-memory indexing and retrieval using [PISA](https://github.com/pisa-engine/pisa)
+         - PyTerrier_T5: [[Github](https://github.com/terrierteam/pyterrier_t5)] - neural reranking: monoT5, duoT5
          - PyTerrier_doc2query: [[Github](https://github.com/terrierteam/pyterrier_doc2query)] - neural augmented indexing
+         - PyTerrier_SPLADE: [[Github](https://github.com/cmacdonald/pyt_splade)] - neural augmented indexing
          - PyTerrier_DeepCT: [[Github](https://github.com/terrierteam/pyterrier_deepct)] - neural augmented indexing
         
         You can see examples of how to use these, including notebooks that run on Google Colab, in the contents of our [ECIR 2021 tutorial](https://github.com/terrier-org/ecir2021tutorial).
         
         # Learning to Rank
         
         Complex learning to rank pipelines, including for learning-to-rank, can be constructed using PyTerrier's operator language. For example, to combine two features and make them available for learning, we can use the `**` operator.
```

### Comparing `python-terrier-0.9.1/README.md` & `python-terrier-0.9.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 1. You need to hava Java installed. Pyjnius/PyTerrier will pick up the location automatically.
 2. `pip install python-terrier`
 
 # Indexing
 
 PyTerrier has a number of useful classes for creating indices:
 
- - You can create an index from TREC formatted collection using TRECCollectionIndexer.    
- - For TXT, PDF, Microsoft Word files, etc files you can use FilesIndexer.
- - For Pandas Dataframe you can use DFIndexer.
- - For any abitrary iterable dictionaries, you can use IterDictIndexer.
+ - You can create an index from TREC formatted collection using [TRECCollectionIndexer](https://pyterrier.readthedocs.io/en/latest/terrier-indexing.html#treccollectionindexer).    
+ - For TXT, PDF, Microsoft Word files, etc files you can use [FilesIndexer](https://pyterrier.readthedocs.io/en/latest/terrier-indexing.html#filesindexer).
+ - For Pandas Dataframe you can use [DFIndexer](https://pyterrier.readthedocs.io/en/latest/terrier-indexing.html#dfindexer).
+ - For any abitrary iterable dictionaries, you can use [IterDictIndexer](https://pyterrier.readthedocs.io/en/latest/terrier-indexing.html#iterdictindexer).
 
 See the [indexing documentation](https://pyterrier.readthedocs.io/en/latest/terrier-indexing.html), or the examples in the [indexing notebook](examples/notebooks/indexing.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/terrier-org/pyterrier/blob/master/examples/notebooks/indexing.ipynb)
 
 # Retrieval and Evaluation
 
 ```python
 topics = pt.io.read_topics(topicsFile)
@@ -65,16 +65,18 @@
 # Neural Reranking and Dense Retrieval
 
 PyTerrier has additional plugins for BERT (through OpenNIR), T5, ColBERT, ANCE, DeepCT and doc2query.
 
  - OpenNIR: [[Github](https://github.com/Georgetown-IR-Lab/OpenNIR)] [[Documentation](https://opennir.net/)]
  - PyTerrier_ANCE: [[Github](https://github.com/terrierteam/pyterrier_ance)] - dense retrieval
  - PyTerrier_ColBERT: [[Github](https://github.com/terrierteam/pyterrier_colbert)] - dense retrieval and/or neural reranking
- - PyTerrier_T5: [[Github](https://github.com/terrierteam/pyterrier_t5)] - neural reranking
+ - PyTerrier_PISA: [[Github](https://github.com/terrierteam/pyterrier_pisa)] - fast in-memory indexing and retrieval using [PISA](https://github.com/pisa-engine/pisa)
+ - PyTerrier_T5: [[Github](https://github.com/terrierteam/pyterrier_t5)] - neural reranking: monoT5, duoT5
  - PyTerrier_doc2query: [[Github](https://github.com/terrierteam/pyterrier_doc2query)] - neural augmented indexing
+ - PyTerrier_SPLADE: [[Github](https://github.com/cmacdonald/pyt_splade)] - neural augmented indexing
  - PyTerrier_DeepCT: [[Github](https://github.com/terrierteam/pyterrier_deepct)] - neural augmented indexing
 
 You can see examples of how to use these, including notebooks that run on Google Colab, in the contents of our [ECIR 2021 tutorial](https://github.com/terrier-org/ecir2021tutorial).
 
 # Learning to Rank
 
 Complex learning to rank pipelines, including for learning-to-rank, can be constructed using PyTerrier's operator language. For example, to combine two features and make them available for learning, we can use the `**` operator.
```

### Comparing `python-terrier-0.9.1/pyterrier/__init__.py` & `python-terrier-0.9.2/pyterrier/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 import os
 
 from .bootstrap import _logging, setup_terrier, setup_jnius, is_windows
 
 # definitive API used by others, now available before pt.init
 from .transformer import Transformer, Estimator, Indexer
```

### Comparing `python-terrier-0.9.1/pyterrier/anserini.py` & `python-terrier-0.9.2/pyterrier/anserini.py`

 * *Files identical despite different names*

### Comparing `python-terrier-0.9.1/pyterrier/apply.py` & `python-terrier-0.9.2/pyterrier/apply.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         Can be used in batch-wise manner, which is particularly useful for appling neural models. In this case,
         the scoring function receives a dataframe, rather than a single row::
 
             def _doclen(df):
                 # returns series of lengths
                 return df.text.str.len()
             
-            pipe = pt.BatchRetrieve(index) >> pt.apply.doc_score(_doclen)
+            pipe = pt.BatchRetrieve(index) >> pt.apply.doc_score(_doclen, batch_size=128)
 
     """
     return ApplyDocumentScoringTransformer(fn, *args, batch_size=batch_size, **kwargs)
 
 def doc_features(fn : Callable[[pd.Series], NDArray[Any]], *args, **kwargs) -> Transformer:
     """
         Create a transformer that takes as input a ranked documents dataframe, and applies the supplied function to each document to compute feature scores. 
@@ -126,40 +126,44 @@
 
         Example::
             
             pipe = pt.BatchRetrieve(index, metadata=["docno", "body"]) >> pt.apply.rename({'body':'text'})
     """
     return ApplyGenericTransformer(lambda df: df.rename(columns=columns), *args, **kwargs)
 
-def generic(fn : Callable[[pd.DataFrame], pd.DataFrame], *args, **kwargs) -> Transformer:
+def generic(fn : Callable[[pd.DataFrame], pd.DataFrame], *args, batch_size=None, **kwargs) -> Transformer:
     """
         Create a transformer that changes the input dataframe to another dataframe in an unspecified way.
 
         The supplied function is called once for an entire result set as a dataframe (which may contain one of more queries).
         Each time it should return a new dataframe. The returned dataframe should abide by the general PyTerrier Data Model,
         for instance updating the rank column if the scores are amended.
 
         Arguments:
             fn(Callable): the function to apply to each row
+            batch_size(int or None): whether to apply fn on batches of rows or all that are received
+            verbose(bool): Whether to display a progress bar over batches (only used if batch_size is set).
 
         Example::
 
             # this transformer will remove all documents at rank greater than 2.
 
             # this pipeline would remove all but the first two documents from a result set
             pipe = pt.BatchRetrieve(index) >> pt.apply.generic(lambda res : res[res["rank"] < 2])
 
     """
-    return ApplyGenericTransformer(fn, *args, **kwargs)
+    return ApplyGenericTransformer(fn, *args, batch_size=batch_size, **kwargs)
 
-def by_query(fn : Callable[[pd.DataFrame], pd.DataFrame], *args, **kwargs) -> Transformer:
+def by_query(fn : Callable[[pd.DataFrame], pd.DataFrame], *args, batch_size=None, **kwargs) -> Transformer:
     """
         As `pt.apply.generic()` except that fn receives a dataframe for one query at at time, rather than all results at once.
+        If batch_size is set, fn will receive no more than batch_size documents for any query. The verbose kwargs controls whether
+        to display a progress bar over queries.  
     """
-    return ApplyForEachQuery(fn, *args, **kwargs)
+    return ApplyForEachQuery(fn, *args, batch_size=batch_size, **kwargs)
 
 class _apply:
 
     def __init__(self):
         _bind(self, lambda self, fn, *args, **kwargs : query(fn, *args, **kwargs), as_name='query')
         _bind(self, lambda self, fn, *args, **kwargs : doc_score(fn, *args, **kwargs), as_name='doc_score')
         _bind(self, lambda self, fn, *args, **kwargs : doc_features(fn, *args, **kwargs), as_name='doc_features')
```

### Comparing `python-terrier-0.9.1/pyterrier/apply_base.py` & `python-terrier-0.9.2/pyterrier/apply_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,35 +12,61 @@
         self.fn = fn
         self.verbose = verbose
 
     def __repr__(self):
         return "pt.apply.??()"
 
 class ApplyForEachQuery(ApplyTransformerBase):
-    def __init__(self, fn,  *args, add_ranks=True, **kwargs):
+    def __init__(self, fn,  *args, add_ranks=True, batch_size=None, **kwargs):
         """
             Arguments:
              - fn (Callable): Takes as input a panda Series for a row representing that document, and returns the new float doument score 
         """
         super().__init__(fn, *args, **kwargs)
         self.add_ranks = add_ranks
+        self.batch_size = batch_size
+    
+    def __repr__(self):
+        return "pt.apply.by_query()"
     
     def transform(self, res):
         if len(res) == 0:
             return self.fn(res)
+
+        import math, pandas as pd
+        from pyterrier.model import split_df
+        from . import tqdm
+
         it = res.groupby("qid")
         if self.verbose:
             it = tqdm(it, unit='query')
         try:
-            dfs = [self.fn(group) for qid, group in it]
-            if self.add_ranks:
-                dfs = [add_ranks(df, single_query=True) for df in dfs]
-            rtr = pd.concat(dfs)
+            if self.batch_size is None:
+                query_dfs = [self.fn(group) for qid, group in it]
+            else:
+                # fn cannot be applied to more than batch_size rows at once
+                # so we must split and reconstruct the output FOR EACH QUERY
+                query_dfs = []
+                for qid, group in it:
+                    
+                    num_chunks = math.ceil( len(group) / self.batch_size )
+                    iterator = split_df(group, num_chunks)
+                    query_dfs.append( pd.concat([self.fn(chunk_df) for chunk_df in iterator]) )
         except Exception as a:
             raise Exception("Problem applying %s" % self.fn) from a
+
+        if self.add_ranks:
+            try:
+                query_dfs = [add_ranks(df, single_query=True) for df in query_dfs]
+            except KeyError as ke:
+                suffix = 'Try setting add_ranks=False'
+                if len(query_dfs) > 0 and 'score' not in query_dfs[0].columns:
+                    suffix = 'Score column not present. Set add_ranks=False'
+                raise ValueError("Cannot apply add_ranks in pt.apply.by_query -" + suffix) from ke
+        rtr = pd.concat(query_dfs)
         return rtr
 
 class ApplyDocumentScoringTransformer(ApplyTransformerBase):
     """
         Implements a transformer that can apply a function to perform document scoring. The supplied function 
         should take as input one row, and return a float for the score of the document.
         
@@ -66,31 +92,41 @@
              - fn (Callable): Takes as input a panda Series for a row representing that document, and returns the new float doument score. If batch_size is set,
              takes a dataframe, and returns a sequence of floats representing scores for those documents.
              - batch_size (int or None). How many documents to operate on at once. If None, operates row-wise
         """
         super().__init__(fn, *args, **kwargs)
         self.batch_size = batch_size
 
+    def __repr__(self):
+        return "pt.apply.doc_score()"
+
     def _transform_rowwise(self, outputRes):
         fn = self.fn
+        if len(outputRes) == 0:
+            outputRes["score"] = pd.Series(dtype='float64')
+            return outputRes
         if self.verbose:
             tqdm.pandas(desc="pt.apply.doc_score", unit="d")
-            outputRes["score"] = outputRes.progress_apply(fn, axis=1)
+            outputRes["score"] = outputRes.progress_apply(fn, axis=1).astype('float64')
         else:
-            outputRes["score"] = outputRes.apply(fn, axis=1)
+            outputRes["score"] = outputRes.apply(fn, axis=1).astype('float64')
         outputRes = add_ranks(outputRes)
         return outputRes
     
     def _transform_batchwise(self, outputRes):
         fn = self.fn
         outputRes["score"] = fn(outputRes)
+        outputRes["score"] = outputRes["score"].astype('float64')
         return outputRes
     
     def transform(self, inputRes):
         outputRes = inputRes.copy()
+        if len(outputRes) == 0:
+            outputRes["score"] = pd.Series(dtype='float64')
+            return add_ranks(outputRes)
         if self.batch_size is None:
             return self._transform_rowwise(inputRes)
 
         import math
         from .model import split_df
         from . import tqdm
         num_chunks = math.ceil( len(inputRes) / self.batch_size )
@@ -115,14 +151,17 @@
     def __init__(self, fn,  *args, **kwargs):
         """
             Arguments:
              - fn (Callable): Takes as input a panda Series for a row representing that document, and returns a new numpy array representing the features of that document
         """
         super().__init__(fn, *args, **kwargs)
 
+    def __repr__(self):
+        return "pt.apply.doc_features()"
+
     def transform(self, inputRes):
         fn = self.fn
         outputRes = inputRes.copy()
         if self.verbose:
             tqdm.pandas(desc="pt.apply.doc_features", unit="d")
             outputRes["features"] = outputRes.progress_apply(fn, axis=1)
         else:
@@ -152,14 +191,17 @@
         """
             Arguments:
              - fn (Callable): Takes as input a panda Series for a row representing a query, and returns the new string query 
              - verbose (bool): Display a tqdm progress bar for this transformer
         """
         super().__init__(fn, *args, **kwargs)
 
+    def __repr__(self):
+        return "pt.apply.query()"
+
     def transform(self, inputRes):
         from .model import push_queries
         fn = self.fn
         outputRes = push_queries(inputRes.copy(), inplace=True, keep_original=True)
         if self.verbose:
             tqdm.pandas(desc="pt.apply.query", unit="d")
             outputRes["query"] = outputRes.progress_apply(fn, axis=1)
@@ -183,18 +225,34 @@
         # this pipeline would remove all but the first two documents from a result set
         lp = ApplyGenericTransformer(lambda res : res[res["rank"] < 2])
 
         pipe = pt.BatchRetrieve(index) >> lp
 
     """
 
-    def __init__(self, fn,  *args, **kwargs):
+    def __init__(self, fn,  *args, batch_size=None, **kwargs):
         """
             Arguments:
              - fn (Callable): Takes as input a panda DataFrame, and returns a new Pandas DataFrame 
         """
         super().__init__(fn, *args, **kwargs)
+        self.batch_size = batch_size
+
+    def __repr__(self):
+        return "pt.apply.generic()"
 
     def transform(self, inputRes):
-        fn = self.fn
-        return fn(inputRes)
+        # no batching
+        if self.batch_size is None:
+            return self.fn(inputRes)
+
+        # batching
+        import math, pandas as pd
+        from pyterrier.model import split_df
+        from . import tqdm
+        num_chunks = math.ceil( len(inputRes) / self.batch_size )
+        iterator = split_df(inputRes, num_chunks)
+        if self.verbose:
+            iterator = tqdm(iterator, desc="pt.apply", unit='row') 
+        rtr = pd.concat([self.fn(chunk_df) for chunk_df in iterator])
+        return rtr
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python-terrier-0.9.1/pyterrier/batchretrieve.py` & `python-terrier-0.9.2/pyterrier/batchretrieve.py`

 * *Files 1% similar despite different names*

```diff
@@ -514,15 +514,15 @@
             # BR and think it is re-ranking. In fact, we only need qid and query
             input = topics
         elif self.takes == "docs":
             # we have to pass the documents, but its desirable to have the docids mapped to the new index already
             # build a mapping, as the metaindex may not have reverse lookups enabled
             input = topics_and_res.copy()
             # add the docid to the dataframe
-            input["docid"] = input.apply(lambda row: docno2docid[row["docno"]], axis=1)
+            input["docid"] = input.apply(lambda row: docno2docid[row["docno"]], axis=1, result_type='reduce')
 
 
         # and then just instantiate BR using the our new index 
         # we take all other arguments as arguments for BR
         inner = self.innerclass(index, **(self.kwargs))
         inner.verbose = self.verbose
         inner_res = inner.transform(input)
```

### Comparing `python-terrier-0.9.1/pyterrier/bootstrap.py` & `python-terrier-0.9.2/pyterrier/bootstrap.py`

 * *Files identical despite different names*

### Comparing `python-terrier-0.9.1/pyterrier/cache.py` & `python-terrier-0.9.2/pyterrier/cache.py`

 * *Files identical despite different names*

### Comparing `python-terrier-0.9.1/pyterrier/datasets.py` & `python-terrier-0.9.2/pyterrier/datasets.py`

 * *Files identical despite different names*

### Comparing `python-terrier-0.9.1/pyterrier/debug.py` & `python-terrier-0.9.2/pyterrier/debug.py`

 * *Files identical despite different names*

### Comparing `python-terrier-0.9.1/pyterrier/index.py` & `python-terrier-0.9.2/pyterrier/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import threading
 import select
 import math
 from warnings import warn
 from deprecated import deprecated
 from collections import deque
 from typing import List, Dict, Union, Any
+import more_itertools
 
 StringReader = None
 HashMap = None
 TaggedDocument = None
 FlatJSONDocument = None
 Tokeniser = None
 TRECCollection = None
@@ -580,15 +581,19 @@
         CLITool.main(["indexutil", "-I" + self.path, util])
 
 
 class DFIndexUtils:
 
     @staticmethod
     def get_column_lengths(df):
-        return dict([(v, df[v].apply(lambda r: len(str(r)) if r!=None else 0).max())for v in df.columns.values])
+        import math
+        meta2len = dict([(v, df[v].apply(lambda r: len(str(r)) if r!=None else 0).max())for v in df.columns.values])
+        # nan values can arise if df is empty. Here we take a metalength of 1 instead.
+        meta2len = {k : 1 if math.isnan(l) else l for k, l in meta2len.items()}
+        return meta2len
 
     @staticmethod
     def create_javaDocIterator(text, *args, **kwargs):
         if HashMap is None:
             run_autoclass()
 
         all_metadata = {}
@@ -609,14 +614,16 @@
             elif isinstance(value, pd.DataFrame):
                 for name, column in arg.items():
                     all_metadata[name] = column
                     assert len(column) == len(text), "Length of metadata arguments needs to be equal to length of text argument"
             else:
                 raise ValueError("Keyword kwargs need to be of type pandas.Series, list or tuple")
 
+        if "docno" not in all_metadata:
+            raise ValueError('No docno column specified, while PyTerrier assumes a docno should exist. Found meta columns were %s' % str(list(all_metadata.keys())))
         # this method creates the documents as and when needed.
         def convertDoc(text_row, meta_column):
             if text_row is None:
                 text_row = ""
             hashmap = HashMap()
             for column, value in meta_column[1].iteritems():
                 if value is None:
@@ -803,21 +810,51 @@
                 'metaindex.compressed.crop.long' : 'true',
                 'FieldTags.process': ','.join(fields),
                 'FieldTags.casesensitive': 'true',
             })
 
     def _filter_iterable(self, it, indexed_fields):
         # Only include necessary fields: those that are indexed, metadata fields, and docno
-        
+        # Also, check that the provided iterator is a suitable format
+
         if self.pretokenised:
             all_fields = {'docno', "toks"} | set(self.meta.keys())
         else:
             all_fields = {'docno'} | set(indexed_fields) | set(self.meta.keys())
-        for doc in it:
-            yield {f: doc[f] for f in all_fields}
+
+        (first_doc,), it = more_itertools.spy(it) # peek at the first document and validate it
+        self._validate_doc_dict(first_doc)
+
+        # important: return an iterator here, rather than make this function a generator,
+        # to be sure that the validation above happens when _filter_iterable is called,
+        # rather than on the first invocation of next()
+        return ({f: doc[f] for f in all_fields} for doc in it)
+
+    def _is_dict(self, obj):
+        return hasattr(obj, '__getitem__') and hasattr(obj, 'items')
+
+    def _validate_doc_dict(self, obj):
+        """
+        Raise errors/warnings for common indexing mistakes
+        """
+        if not self._is_dict(obj):
+            raise ValueError("Was passed %s while expected dict-like object" % (str(type(obj))))
+        if self.meta is not None:
+            for k in self.meta:
+                if k not in obj:
+                    raise ValueError(f"Indexing meta key {k} not found in first document (keys {list(obj.keys())})")
+                if len(obj) > int(self.meta[k]):
+                    msg = f"Indexing meta key {k} length requested {self.meta[k]} but exceeded in first document (actual length {len(obj[k])}). " + \
+                          f"Increase the length in the meta dict for the indexer, e.g., pt.IterDictIndexer(..., meta={ {k: len(obj[k])} })."
+                    if k == 'docno':
+                        # docnos that are truncated will cause major issues; raise an error
+                        raise ValueError(msg)
+                    else:
+                        # Other fields may not matter as much; just show a warning
+                        warn(msg)
 
 
 class _IterDictIndexer_nofifo(_BaseIterDictIndexer):
     """
     Use this Indexer if you wish to index an iter of dicts (possibly with multiple fields).
     This version is used for Windows -- which doesn't support the faster fifo implementation.
     """
@@ -845,15 +882,15 @@
             assert not self.blocks, "pretokenised isnt compatible with blocks"
 
             # we generate DocumentPostingList from a dictionary of pretokenised text, e.g.
             # [
             #     {'docno' : 'd1', 'toks' : {'a' : 1, 'aa' : 2}}
             # ]
             
-            iter_docs = DocListIterator(it)
+            iter_docs = DocListIterator(self._filter_iterable(it, fields))
             self.index_called = True
             index.indexDocuments(iter_docs)
             iter_docs = None
 
         else:
 
             # we need to prevent collectionIterator from being GCd
```

### Comparing `python-terrier-0.9.1/pyterrier/io.py` & `python-terrier-0.9.2/pyterrier/io.py`

 * *Files identical despite different names*

### Comparing `python-terrier-0.9.1/pyterrier/ltr.py` & `python-terrier-0.9.2/pyterrier/ltr.py`

 * *Files identical despite different names*

### Comparing `python-terrier-0.9.1/pyterrier/mavenresolver.py` & `python-terrier-0.9.2/pyterrier/mavenresolver.py`

 * *Files identical despite different names*

### Comparing `python-terrier-0.9.1/pyterrier/model.py` & `python-terrier-0.9.2/pyterrier/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
         for each query. Note that the dataframe is NOT sorted by this operation (this is defined by STRICT_SORT).
         The dataframe is modified, i.e. inplace.
 
         Arguments
             df: dataframe to create rank attribute for
             single_query (bool): whether the dataframe contains only a single-query or not. This method will be quicker for single-query dataframes
     """
-
+    if "score" not in df.columns:
+        raise KeyError("Must have score column to add ranks to dataframe. Found columns were %s" % str(df.columns.values.tolist()))
     df.drop(columns=["rank"], errors="ignore", inplace=True)
     if len(df) == 0:
         df["rank"] = pd.Series(index=df.index, dtype='int64')
         return df
 
     # remove group when single_query is True
     if single_query:
```

### Comparing `python-terrier-0.9.1/pyterrier/new.py` & `python-terrier-0.9.2/pyterrier/new.py`

 * *Files identical despite different names*

### Comparing `python-terrier-0.9.1/pyterrier/ops.py` & `python-terrier-0.9.2/pyterrier/ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .transformer import Transformer, Estimator, get_transformer, Scalar
 from .model import add_ranks
 from matchpy import Operation, Arity
 from warnings import warn
-from typing import Iterable, Iterator, Union
+from typing import Iterable
+import pandas as pd
 
 class BinaryTransformerBase(Transformer,Operation):
     """
         A base class for all operator transformers that can combine the input of exactly 2 transformers. 
     """
     arity = Arity.binary
 
@@ -220,15 +221,15 @@
                 "should not contain a features column; found columns were %s" %  str(inputRes.columns))
         
         all_results = []
 
         for i, m in enumerate(self.models):
             #IMPORTANT this .copy() is important, in case an operand transformer changes inputRes
             results = m.transform(inputRes.copy())
-            if len(results) == 0:
+            if len(results) == 0 and num_results != 0:
                 raise ValueError("Got no results from %s, expected %d" % (repr(m), num_results) )
             assert not "features_x" in results.columns 
             assert not "features_y" in results.columns
             all_results.append( results )
 
     
         for i, (m, res) in enumerate(zip(self.models, all_results)):
@@ -239,15 +240,18 @@
 
                 if len(res) != num_results:
                     warn("Got number of results different expected from %s, expected %d received %d, feature scores for any "
                         "missing documents be 0, extraneous documents will be removed" % (repr(m), num_results, len(res)))
                     all_results[i] = res = inputRes[["qid", "docno"]].merge(res, on=["qid", "docno"], how="left")
                     res["score"] = res["score"].fillna(value=0)
 
-                res["features"] = res.apply(lambda row : np.array([row["score"]]), axis=1)
+                if len(res) == 0:
+                    res["features"] = pd.Series([], dtype='float64')
+                else:
+                    res["features"] = res.apply(lambda row : np.array([row["score"]]), axis=1)
                 res.drop(columns=["score"], inplace=True)
             assert "features" in res.columns
             #print("%d got %d features from operand %d" % ( id(self) ,   len(results.iloc[0]["features"]), i))
 
         def _concat_features(row):
             assert isinstance(row["features_x"], np.ndarray)
             assert isinstance(row["features_y"], np.ndarray)
@@ -258,16 +262,16 @@
         
         def _reduce_fn(left, right):
             import pandas as pd
             both_cols = set(left.columns) & set(right.columns)
             both_cols.remove("qid")
             both_cols.remove("docno")
             both_cols.remove("features")
-            rtr = pd.merge(left, right, on=["qid", "docno"])            
-            rtr["features"] = rtr.apply(_concat_features, axis=1)
+            rtr = pd.merge(left, right, on=["qid", "docno"])
+            rtr["features"] = rtr.apply(_concat_features, axis=1, result_type='reduce')
             rtr.rename(columns={"%s_x" % col : col for col in both_cols}, inplace=True)
             rtr.drop(columns=["features_x", "features_y"] + ["%s_y" % col for col in both_cols], inplace=True)
             return rtr
         
         from functools import reduce
         final_DF = reduce(_reduce_fn, all_results)
```

### Comparing `python-terrier-0.9.1/pyterrier/parallel.py` & `python-terrier-0.9.2/pyterrier/parallel.py`

 * *Files identical despite different names*

### Comparing `python-terrier-0.9.1/pyterrier/pipelines.py` & `python-terrier-0.9.2/pyterrier/pipelines.py`

 * *Files identical despite different names*

### Comparing `python-terrier-0.9.1/pyterrier/rewrite.py` & `python-terrier-0.9.2/pyterrier/rewrite.py`

 * *Files identical despite different names*

### Comparing `python-terrier-0.9.1/pyterrier/text.py` & `python-terrier-0.9.2/pyterrier/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,19 @@
     def add_docids(res):
         res = res.copy()
         res["docid"] = res.apply(lambda row: metaindex.getDocument("docno", row.docno), axis=1)
         return res
 
     def add_text_function_docids(res):
         res = res.copy()
+        if len(res) == 0:
+            for k in metadata:
+                res[k] = pd.Series(dtype='object')
+            return res
+
         docids = res.docid.values.tolist()
         # indexed by docid then keys
         allmeta = metaindex.getItems(metadata, docids)
         import numpy as np
         # get transpose to make easier for insertion back into dataframe?
         allmeta = np.array(allmeta).T
         for i, k in enumerate(metadata):
```

### Comparing `python-terrier-0.9.1/pyterrier/transformer.py` & `python-terrier-0.9.2/pyterrier/transformer.py`

 * *Files identical despite different names*

### Comparing `python-terrier-0.9.1/pyterrier/utils.py` & `python-terrier-0.9.2/pyterrier/utils.py`

 * *Files identical despite different names*

### Comparing `python-terrier-0.9.1/python_terrier.egg-info/PKG-INFO` & `python-terrier-0.9.2/python_terrier.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-terrier
-Version: 0.9.1
+Version: 0.9.2
 Summary: Terrier IR platform Python API
 Home-page: https://github.com/terrier-org/pyterrier
 Author: Craig Macdonald
 Author-email: craigm@dcs.gla.ac.uk
 License: UNKNOWN
 Description: ![Python package](https://github.com/terrier-org/pyterrier/workflows/Python%20package/badge.svg) 
         [![PyPI version](https://badge.fury.io/py/python-terrier.svg)](https://badge.fury.io/py/python-terrier)
@@ -28,18 +28,18 @@
         1. You need to hava Java installed. Pyjnius/PyTerrier will pick up the location automatically.
         2. `pip install python-terrier`
         
         # Indexing
         
         PyTerrier has a number of useful classes for creating indices:
         
-         - You can create an index from TREC formatted collection using TRECCollectionIndexer.    
-         - For TXT, PDF, Microsoft Word files, etc files you can use FilesIndexer.
-         - For Pandas Dataframe you can use DFIndexer.
-         - For any abitrary iterable dictionaries, you can use IterDictIndexer.
+         - You can create an index from TREC formatted collection using [TRECCollectionIndexer](https://pyterrier.readthedocs.io/en/latest/terrier-indexing.html#treccollectionindexer).    
+         - For TXT, PDF, Microsoft Word files, etc files you can use [FilesIndexer](https://pyterrier.readthedocs.io/en/latest/terrier-indexing.html#filesindexer).
+         - For Pandas Dataframe you can use [DFIndexer](https://pyterrier.readthedocs.io/en/latest/terrier-indexing.html#dfindexer).
+         - For any abitrary iterable dictionaries, you can use [IterDictIndexer](https://pyterrier.readthedocs.io/en/latest/terrier-indexing.html#iterdictindexer).
         
         See the [indexing documentation](https://pyterrier.readthedocs.io/en/latest/terrier-indexing.html), or the examples in the [indexing notebook](examples/notebooks/indexing.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/terrier-org/pyterrier/blob/master/examples/notebooks/indexing.ipynb)
         
         # Retrieval and Evaluation
         
         ```python
         topics = pt.io.read_topics(topicsFile)
@@ -73,16 +73,18 @@
         # Neural Reranking and Dense Retrieval
         
         PyTerrier has additional plugins for BERT (through OpenNIR), T5, ColBERT, ANCE, DeepCT and doc2query.
         
          - OpenNIR: [[Github](https://github.com/Georgetown-IR-Lab/OpenNIR)] [[Documentation](https://opennir.net/)]
          - PyTerrier_ANCE: [[Github](https://github.com/terrierteam/pyterrier_ance)] - dense retrieval
          - PyTerrier_ColBERT: [[Github](https://github.com/terrierteam/pyterrier_colbert)] - dense retrieval and/or neural reranking
-         - PyTerrier_T5: [[Github](https://github.com/terrierteam/pyterrier_t5)] - neural reranking
+         - PyTerrier_PISA: [[Github](https://github.com/terrierteam/pyterrier_pisa)] - fast in-memory indexing and retrieval using [PISA](https://github.com/pisa-engine/pisa)
+         - PyTerrier_T5: [[Github](https://github.com/terrierteam/pyterrier_t5)] - neural reranking: monoT5, duoT5
          - PyTerrier_doc2query: [[Github](https://github.com/terrierteam/pyterrier_doc2query)] - neural augmented indexing
+         - PyTerrier_SPLADE: [[Github](https://github.com/cmacdonald/pyt_splade)] - neural augmented indexing
          - PyTerrier_DeepCT: [[Github](https://github.com/terrierteam/pyterrier_deepct)] - neural augmented indexing
         
         You can see examples of how to use these, including notebooks that run on Google Colab, in the contents of our [ECIR 2021 tutorial](https://github.com/terrier-org/ecir2021tutorial).
         
         # Learning to Rank
         
         Complex learning to rank pipelines, including for learning-to-rank, can be constructed using PyTerrier's operator language. For example, to combine two features and make them available for learning, we can use the `**` operator.
```

### Comparing `python-terrier-0.9.1/python_terrier.egg-info/SOURCES.txt` & `python-terrier-0.9.2/python_terrier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-terrier-0.9.1/setup.py` & `python-terrier-0.9.2/setup.py`

 * *Files identical despite different names*

