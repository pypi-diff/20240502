# Comparing `tmp/twembeddings-0.1.tar.gz` & `tmp/twembeddings-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/twembeddings-0.1.tar", last modified: Fri Jun 17 15:09:48 2022, max compression
+gzip compressed data, was "/home/bmazoyer/Dev/twembeddings/dist/.tmp-cq1en_hh/twembeddings-0.2.0.tar", last modified: Thu May  2 14:45:13 2024, max compression
```

## Comparing `twembeddings-0.1.tar` & `twembeddings-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2022-06-17 15:09:48.782415 twembeddings-0.1/
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     1091 2020-09-17 14:29:09.000000 twembeddings-0.1/LICENSE
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      247 2022-06-17 15:09:48.782415 twembeddings-0.1/PKG-INFO
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    12898 2021-04-15 15:07:17.000000 twembeddings-0.1/README.md
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)       38 2022-06-17 15:09:48.782415 twembeddings-0.1/setup.cfg
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      713 2022-06-17 15:07:24.000000 twembeddings-0.1/setup.py
-drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2022-06-17 15:09:48.782415 twembeddings-0.1/twembeddings/
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      228 2021-11-03 13:45:54.000000 twembeddings-0.1/twembeddings/__init__.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    17370 2022-06-17 15:04:34.000000 twembeddings-0.1/twembeddings/build_features_matrix.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     7524 2021-05-26 16:01:17.000000 twembeddings-0.1/twembeddings/clustering_algo.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    14879 2022-06-17 15:04:34.000000 twembeddings-0.1/twembeddings/embeddings.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     5813 2021-05-26 12:08:02.000000 twembeddings-0.1/twembeddings/eval.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     5354 2020-09-17 14:29:09.000000 twembeddings-0.1/twembeddings/stop_words.py
-drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2022-06-17 15:09:48.782415 twembeddings-0.1/twembeddings.egg-info/
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      247 2022-06-17 15:09:48.000000 twembeddings-0.1/twembeddings.egg-info/PKG-INFO
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      410 2022-06-17 15:09:48.000000 twembeddings-0.1/twembeddings.egg-info/SOURCES.txt
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)        1 2022-06-17 15:09:48.000000 twembeddings-0.1/twembeddings.egg-info/dependency_links.txt
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)        1 2021-07-06 12:38:22.000000 twembeddings-0.1/twembeddings.egg-info/not-zip-safe
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      173 2022-06-17 15:09:48.000000 twembeddings-0.1/twembeddings.egg-info/requires.txt
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)       13 2022-06-17 15:09:48.000000 twembeddings-0.1/twembeddings.egg-info/top_level.txt
+drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2024-05-02 14:45:13.882924 twembeddings-0.2.0/
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     1091 2020-09-17 14:29:09.000000 twembeddings-0.2.0/LICENSE
+-rw-r--r--   0 bmazoyer  (1000) bmazoyer  (1000)      666 2024-05-02 14:45:13.882924 twembeddings-0.2.0/PKG-INFO
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    12898 2021-04-15 15:07:17.000000 twembeddings-0.2.0/README.md
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)       38 2024-05-02 14:45:13.882924 twembeddings-0.2.0/setup.cfg
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      734 2024-05-02 14:44:36.000000 twembeddings-0.2.0/setup.py
+drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2024-05-02 14:45:13.882924 twembeddings-0.2.0/twembeddings/
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      228 2021-11-03 13:45:54.000000 twembeddings-0.2.0/twembeddings/__init__.py
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    17883 2024-05-02 14:28:24.000000 twembeddings-0.2.0/twembeddings/build_features_matrix.py
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     7524 2021-05-26 16:01:17.000000 twembeddings-0.2.0/twembeddings/clustering_algo.py
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    14145 2023-11-22 15:48:23.000000 twembeddings-0.2.0/twembeddings/embeddings.py
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     5813 2021-05-26 12:08:02.000000 twembeddings-0.2.0/twembeddings/eval.py
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     5354 2020-09-17 14:29:09.000000 twembeddings-0.2.0/twembeddings/stop_words.py
+drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2024-05-02 14:45:13.882924 twembeddings-0.2.0/twembeddings.egg-info/
+-rw-r--r--   0 bmazoyer  (1000) bmazoyer  (1000)      666 2024-05-02 14:45:13.000000 twembeddings-0.2.0/twembeddings.egg-info/PKG-INFO
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      410 2024-05-02 14:45:13.000000 twembeddings-0.2.0/twembeddings.egg-info/SOURCES.txt
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)        1 2024-05-02 14:45:13.000000 twembeddings-0.2.0/twembeddings.egg-info/dependency_links.txt
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)        1 2021-07-06 12:38:22.000000 twembeddings-0.2.0/twembeddings.egg-info/not-zip-safe
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      192 2024-05-02 14:45:13.000000 twembeddings-0.2.0/twembeddings.egg-info/requires.txt
+-rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)       13 2024-05-02 14:45:13.000000 twembeddings-0.2.0/twembeddings.egg-info/top_level.txt
```

### Comparing `twembeddings-0.1/LICENSE` & `twembeddings-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twembeddings-0.1/README.md` & `twembeddings-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `twembeddings-0.1/twembeddings/build_features_matrix.py` & `twembeddings-0.2.0/twembeddings/build_features_matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 from .embeddings import TOKEN_PATTERN
 from .stop_words import STOP_WORDS_FR, STOP_WORDS_EN
 from scipy.sparse import issparse, save_npz, load_npz
 import numpy as np
 import os
 import re
 import csv
+import tensorflow_hub as hub
 from unidecode import unidecode
 from datetime import datetime, timedelta
 from collections import deque, defaultdict
 import math
 
 __all__ = ['build_matrix', 'load_dataset', 'load_matrix', 'save_tokens_JLH']
 
 TWITTER_DATE_FORMAT = "%a %b %d %H:%M:%S +0000 %Y"
 STANDARD_DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 logging.basicConfig(format='%(asctime)s - %(levelname)s : %(message)s', level=logging.INFO)
 text_embeddings = ['tfidf_all_tweets', 'tfidf_dataset', 'w2v_afp_fr', 'w2v_gnews_en', 'w2v_twitter_fr',
-                   "w2v_twitter_en", "elmo", "bert", "bert_tweets", "sbert_sts", "sbert_stsshort",
+                   "w2v_twitter_en", "elmo", "bert", "bert_tweets", "sbert", "sbert_sts", "sbert_stsshort",
                    "sbert_tweets_sts", "sbert_nli_sts", "sbert_tweets_sts_long", "use_multilingual", "use"]
 image_embeddings = ["resnet", "densenet"]
 
 
 def strp_date_created_at(created_at):
     if "+0000" in created_at:
         return datetime.strptime(created_at, TWITTER_DATE_FORMAT)
@@ -83,14 +84,17 @@
     else:
         dataset = args["dataset"].split("/")[-1].replace(".tsv", "")
 
     file_name = args["annotation"]
     for arg in ["text+", "hashtag_split", "svd", "tfidf_weights"]:
         if args[arg]:
             file_name += "_" + arg
+    if args["model"] == "sbert":
+        sbert_model = args["sub_model"].split("/")[-1]
+        file_name += "_" + sbert_model
     return os.path.join("data", dataset, args["model"], file_name)
 
 
 def save_matrix(X, **args):
     path = build_path(**args)
     os.makedirs(os.path.join(*path.split("/")[:-1]), exist_ok=True)
     if issparse(X):
@@ -302,25 +306,33 @@
     elif args["model"].startswith("sbert"):
         data.text = data.text.apply(format_text,
                                     remove_mentions=args["remove_mentions"],
                                     unidecode=False,
                                     lower=False,
                                     hashtag_split=True
                                     )
-        vectorizer = SBERT(lang=args["lang"])
+
+        vectorizer = SBERT(sbert_model=args["sub_model"])
         X = vectorizer.compute_vectors(data)
 
     elif args["model"].startswith("use"):
         data.text = data.text.apply(format_text,
                                     remove_mentions=args["remove_mentions"],
                                     unidecode=False,
                                     lower=False,
                                     hashtag_split=True
                                     )
-        vectorizer = USE()
+
+        # todo: prevent warning message if no cuda with os.environ['CUDA_VISIBLE_DEVICES'] = '-1'
+        if args["lang"] == "en":
+            embed = hub.load("https://tfhub.dev/google/universal-sentence-encoder-large/5")
+        else:
+            embed = hub.load("https://tfhub.dev/google/universal-sentence-encoder-multilingual/3")
+
+        vectorizer = USE(embed)
         X = vectorizer.compute_vectors(data)
 
     elif args["model"] == "resnet":
         vectorizer = ResNetLayer()
         X = vectorizer.compute_vectors("data/images/event2018_image/")
 
     elif args["model"] == "densenet":
@@ -335,15 +347,15 @@
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument('--dataset',
                         required=False,
                         default="event2018",
                         help="""
-                            - 'event2018' : Event2018 dataset;  
+                            - 'event2018' : Event2018 dataset;
                             - 'event2018_image' : all tweets in Event2018 that contain an image. We include tweets that
                         quote an image or reply to an image;
                             - any other value should be the path to your own dataset in tsv format;
                         """)
     parser.add_argument('--model',
                         nargs='+',
                         required=True,
@@ -356,22 +368,22 @@
                         action="store_true",
                         help="""
                         Save the matrix on disk (.npy format for dense matrix, .npz for sparse matrix)
                         """)
     parser.add_argument("--svd", dest="svd", default=False,
                         action="store_true",
                         help="""
-                        Only for TfIdf embedding: create a dense matrix of shape (n_documents, 100) 
+                        Only for TfIdf embedding: create a dense matrix of shape (n_documents, 100)
                         using Singular Value Decomposition
                         """)
     parser.add_argument('--binary', dest="binary", default=True,
                         action="store_false",
                         help="""
-                        Only for TfIdf embedding: if True, all non-zero term counts are set to 1. 
-                        This does not mean outputs will have only 0/1 values, only that the tf term 
+                        Only for TfIdf embedding: if True, all non-zero term counts are set to 1.
+                        This does not mean outputs will have only 0/1 values, only that the tf term
                         in tf-idf is binary.
                         """)
 
     parser.add_argument("--hashtag_split", dest="hashtag_split", default=False,
                         action="store_true",
                         help="""
                         Split hashtags into words on capital letters (#FollowFriday --> Follow Friday)
@@ -383,24 +395,24 @@
                         its tfidf weight
                         """)
     parser.add_argument('--text+',
                         dest="text+", default=False,
                         action="store_true",
                         help="""
                         Only if --dataset argument is set to "event2018" or "event2018_image"
-                        Use the text of the tweet + the text of the tweet quoted or replied to 
+                        Use the text of the tweet + the text of the tweet quoted or replied to
                         """)
     parser.add_argument('--annotation',
                         required=False,
                         default="annotated",
                         choices=["annotated", "examined"],
                         help="""
                         Only if --dataset argument is set to "default" or "has_image"
-                            - annotated : (default) all tweets annotated as related to an event; 
-                            - examined : all tweets annotated as related or unrelated to an event; 
+                            - annotated : (default) all tweets annotated as related to an event;
+                            - examined : all tweets annotated as related or unrelated to an event;
                         """
                         # - no : all tweets in the dataset regardless of annotation
                         )
     parser.add_argument('--lang',
                         required=False,
                         default="fr",
                         choices=["fr", "en"]
```

### Comparing `twembeddings-0.1/twembeddings/clustering_algo.py` & `twembeddings-0.2.0/twembeddings/clustering_algo.py`

 * *Files identical despite different names*

### Comparing `twembeddings-0.1/twembeddings/embeddings.py` & `twembeddings-0.2.0/twembeddings/embeddings.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         features_set = set(self.features_names)
         fit_model = CountVectorizer(stop_words=self.stop_words, tokenizer=self.tokenizer)
         # see https://towardsdatascience.com/hacking-scikit-learns-vectorizers-9ef26a7170af for custom analyzr/tokenizr
         if self.no_pandas:
             fit_model.fit(data)
         else:
             fit_model.fit(data["text"].tolist())
-        for term in fit_model.get_feature_names():
+        for term in fit_model.get_feature_names_out():
             if term not in features_set:
                 self.features_names.append(term)
 
     def build_count_vectors(self, data):
         # sort words following features_name order, absent words will be counted as 0
         count_model = CountVectorizer(binary=self.binary, vocabulary=self.features_names, tokenizer=self.tokenizer)
         if self.no_pandas:
@@ -219,24 +219,17 @@
         data["text"] = data.text.str.slice(0, 500)
         vectors = self.bc.encode(data.text.tolist())
         return vectors
 
 
 class SBERT:
 
-    def __init__(self, lang="fr"):
+    def __init__(self, sbert_model="paraphrase-MiniLM-L12-v2"):
         from sentence_transformers import SentenceTransformer
-        self.name = "SBERT"
-        if lang == "fr":
-            self.model = SentenceTransformer(
-                "/home/bmazoyer/Dev/pytorch_bert/output/sts_fr_long_multilingual_bert-2019-10-01_15-07-03")
-        elif lang == "en":
-            self.model = SentenceTransformer(
-                "bert-large-nli-stsb-mean-tokens"
-            )
+        self.model = SentenceTransformer(sbert_model)
 
     def compute_vectors(self, data):
         data["text"] = data.text.str.slice(0, 500)
         vectors = np.array(self.model.encode(data.text.tolist()))
         return vectors
 
 
@@ -276,44 +269,35 @@
                 )
             return self.vectors
 
 
 class USE:
 
     def __init__(self, lang="fr"):
-        import tensorflow as tf
+
         import tensorflow_hub as hub
-        import tf_sentencepiece
+        # tensorflow_text seems unused but necessary to run the hub.load
+        import tensorflow_text
+
         self.name = "UniversalSentenceEncoder"
-        # Graph set up.
-        g = tf.Graph()
-        with g.as_default():
-            self.text_input = tf.placeholder(dtype=tf.string, shape=[None])
-            if lang == "fr":
-                logging.info(lang)
-                embed = hub.Module("https://tfhub.dev/google/universal-sentence-encoder-multilingual/1")
-            elif lang == "en":
-                logging.info(lang)
-                embed = hub.Module("https://tfhub.dev/google/universal-sentence-encoder-large/3")
-            self.embedded_text = embed(self.text_input)
-            init_op = tf.group([tf.global_variables_initializer(), tf.tables_initializer()])
-        g.finalize()
-
-        # Initialize session.
-        self.session = tf.Session(graph=g)
-        self.session.run(init_op)
+
+        # todo: prevent warning message if no cuda with os.environ['CUDA_VISIBLE_DEVICES'] = '-1'
+        if lang == "en":
+            self.embed = hub.load("https://tfhub.dev/google/universal-sentence-encoder-large/5")
+        else:
+            self.embed = hub.load("https://tfhub.dev/google/universal-sentence-encoder-multilingual/3")
+
+
 
     def compute_vectors(self, data):
         batch_size = 64
         n = data.shape[0]
         vectors = np.zeros([n, 512])
         for i in tqdm(range(0, n, batch_size)):
-            vectors[i:min(n, i+batch_size)] = self.session.run(
-                self.embedded_text,
-                feed_dict={self.text_input: data.text[i:min(n, i+batch_size)].tolist()})
+            vectors[i:min(n, i+batch_size)] = self.embed(data.text[i:min(n, i+batch_size)])
         return vectors
 
 
 class DenseNetLayer:
 
     def __init__(self):
         from keras.models import Model
```

### Comparing `twembeddings-0.1/twembeddings/eval.py` & `twembeddings-0.2.0/twembeddings/eval.py`

 * *Files identical despite different names*

### Comparing `twembeddings-0.1/twembeddings/stop_words.py` & `twembeddings-0.2.0/twembeddings/stop_words.py`

 * *Files identical despite different names*

