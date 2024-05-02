# Comparing `tmp/embtechx-1.0.6.tar.gz` & `tmp/embtechx-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embtechx-1.0.6.tar", last modified: Fri Apr 26 09:11:06 2024, max compression
+gzip compressed data, was "embtechx-1.0.7.tar", last modified: Thu May  2 03:59:00 2024, max compression
```

## Comparing `embtechx-1.0.6.tar` & `embtechx-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-26 09:11:06.220324 embtechx-1.0.6/
--rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-04-26 09:11:06.219388 embtechx-1.0.6/PKG-INFO
-drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-26 09:11:06.212107 embtechx-1.0.6/embtechx/
--rw-r--r--   0 ninananakorn   (501) staff       (20)      860 2024-04-26 09:10:00.000000 embtechx-1.0.6/embtechx/__init__.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     3126 2024-04-26 09:10:05.000000 embtechx-1.0.6/embtechx/dataframe.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     2445 2024-04-26 09:10:07.000000 embtechx-1.0.6/embtechx/domain_emb.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     7381 2024-04-26 09:10:50.000000 embtechx-1.0.6/embtechx/embedding.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     8300 2024-04-26 09:10:40.000000 embtechx-1.0.6/embtechx/evaluate.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     2184 2024-04-26 09:10:46.000000 embtechx-1.0.6/embtechx/search.py
-drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-26 09:11:06.218671 embtechx-1.0.6/embtechx.egg-info/
--rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-04-26 09:11:06.000000 embtechx-1.0.6/embtechx.egg-info/PKG-INFO
--rw-r--r--   0 ninananakorn   (501) staff       (20)      295 2024-04-26 09:11:06.000000 embtechx-1.0.6/embtechx.egg-info/SOURCES.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)        1 2024-04-26 09:11:06.000000 embtechx-1.0.6/embtechx.egg-info/dependency_links.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)       86 2024-04-26 09:11:06.000000 embtechx-1.0.6/embtechx.egg-info/requires.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)        9 2024-04-26 09:11:06.000000 embtechx-1.0.6/embtechx.egg-info/top_level.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)       38 2024-04-26 09:11:06.220415 embtechx-1.0.6/setup.cfg
--rw-r--r--   0 ninananakorn   (501) staff       (20)      364 2024-04-26 09:10:02.000000 embtechx-1.0.6/setup.py
+drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-05-02 03:59:00.312848 embtechx-1.0.7/
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-05-02 03:59:00.312252 embtechx-1.0.7/PKG-INFO
+drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-05-02 03:59:00.302503 embtechx-1.0.7/embtechx/
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      860 2024-05-02 03:52:37.000000 embtechx-1.0.7/embtechx/__init__.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     3182 2024-05-02 03:39:50.000000 embtechx-1.0.7/embtechx/dataframe.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     2445 2024-05-02 03:39:49.000000 embtechx-1.0.7/embtechx/domain_emb.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     7424 2024-05-02 03:39:46.000000 embtechx-1.0.7/embtechx/embedding.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     8300 2024-05-02 03:39:49.000000 embtechx-1.0.7/embtechx/evaluate.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     2184 2024-05-02 03:39:48.000000 embtechx-1.0.7/embtechx/search.py
+drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-05-02 03:59:00.311808 embtechx-1.0.7/embtechx.egg-info/
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-05-02 03:59:00.000000 embtechx-1.0.7/embtechx.egg-info/PKG-INFO
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      295 2024-05-02 03:59:00.000000 embtechx-1.0.7/embtechx.egg-info/SOURCES.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)        1 2024-05-02 03:59:00.000000 embtechx-1.0.7/embtechx.egg-info/dependency_links.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)       86 2024-05-02 03:59:00.000000 embtechx-1.0.7/embtechx.egg-info/requires.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)        9 2024-05-02 03:59:00.000000 embtechx-1.0.7/embtechx.egg-info/top_level.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)       38 2024-05-02 03:59:00.312911 embtechx-1.0.7/setup.cfg
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      364 2024-05-02 03:39:51.000000 embtechx-1.0.7/setup.py
```

### Comparing `embtechx-1.0.6/embtechx/__init__.py` & `embtechx-1.0.7/embtechx/__init__.py`

 * *Files identical despite different names*

### Comparing `embtechx-1.0.6/embtechx/dataframe.py` & `embtechx-1.0.7/embtechx/dataframe.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 class emb_dataframe:
     def create_df(domain_name, file_path):
         if file_path.endswith(".txt"):
             with open(file_path, 'r') as file:
                 corpus = file.read()
                 file.close()
 
+            # detect the language of an imported corpus
             detected_language = detect(corpus)
             if detected_language == ("en"):
                 file = corpus.split(".")
             elif detected_language == ("th"):
                 file = corpus.split(" ")
             else:
                 print("Please import an English or Thai corpus.")
```

### Comparing `embtechx-1.0.6/embtechx/domain_emb.py` & `embtechx-1.0.7/embtechx/domain_emb.py`

 * *Files identical despite different names*

### Comparing `embtechx-1.0.6/embtechx/embedding.py` & `embtechx-1.0.7/embtechx/embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pandas as pd
 from langdetect import *
 
 from .dataframe import emb_dataframe
 concat_df = emb_dataframe.concat_df
 
 model_en = SentenceTransformer("sentence-transformers/all-MiniLM-L6-v2")
-model_th = SentenceTransformer("mrp/simcse-model-m-bert-thai-cased")
+model_th = SentenceTransformer("sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2")
 
 class emb_train:
     def detect_df_language(dataframe):
         df = dataframe.copy()
         sentences = df["Text"].tolist()
         languages = []
         for i in range(len(sentences)):
@@ -58,21 +58,21 @@
         train_list = [anc, pos, neg]
         train = concat_df(train_list)
 
         test_list = [test_domain, test_misc]
         test = concat_df(test_list)
         return test, train
 
-    # train the model (only)
+    # train the model
     def train_model_only(dataframe, file_path):
         # detect the language of the dataframe
         detected_language = emb_train.detect_df_language(dataframe)
         if detected_language == ("th"):
             model = model_th
-            print("Model: mrp/simcse-model-m-bert-thai-cased")
+            print("Model: sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2")
         else:
             model = model_en
             print("Model: sentence-transformers/all-MiniLM-L6-v2")
 
         file_path_before = file_path + "/before"
         file_path_after = file_path + "/after"
```

### Comparing `embtechx-1.0.6/embtechx/evaluate.py` & `embtechx-1.0.7/embtechx/evaluate.py`

 * *Files identical despite different names*

### Comparing `embtechx-1.0.6/embtechx/search.py` & `embtechx-1.0.7/embtechx/search.py`

 * *Files identical despite different names*

