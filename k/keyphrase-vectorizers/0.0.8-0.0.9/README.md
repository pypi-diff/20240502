# Comparing `tmp/keyphrase-vectorizers-0.0.8.tar.gz` & `tmp/keyphrase-vectorizers-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyphrase-vectorizers-0.0.8.tar", last modified: Mon May 16 15:03:08 2022, max compression
+gzip compressed data, was "keyphrase-vectorizers-0.0.9.tar", last modified: Sat Jun 18 19:13:00 2022, max compression
```

## Comparing `keyphrase-vectorizers-0.0.8.tar` & `keyphrase-vectorizers-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2022-05-16 15:03:08.730390 keyphrase-vectorizers-0.0.8/
--rw-r--r--   0 tim        (501) staff       (20)     1518 2022-01-24 16:04:38.000000 keyphrase-vectorizers-0.0.8/LICENSE
--rw-r--r--   0 tim        (501) staff       (20)    25357 2022-05-16 15:03:08.730035 keyphrase-vectorizers-0.0.8/PKG-INFO
--rw-r--r--   0 tim        (501) staff       (20)    24446 2022-05-16 14:58:09.000000 keyphrase-vectorizers-0.0.8/README.md
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2022-05-16 15:03:08.726811 keyphrase-vectorizers-0.0.8/keyphrase_vectorizers/
--rw-r--r--   0 tim        (501) staff       (20)      314 2022-02-01 16:42:11.000000 keyphrase-vectorizers-0.0.8/keyphrase_vectorizers/__init__.py
--rw-r--r--   0 tim        (501) staff       (20)       22 2022-05-16 13:55:30.000000 keyphrase-vectorizers-0.0.8/keyphrase_vectorizers/_version.py
--rw-r--r--   0 tim        (501) staff       (20)    13516 2022-05-16 14:09:11.000000 keyphrase-vectorizers-0.0.8/keyphrase_vectorizers/keyphrase_count_vectorizer.py
--rw-r--r--   0 tim        (501) staff       (20)    11136 2022-05-16 14:08:17.000000 keyphrase-vectorizers-0.0.8/keyphrase_vectorizers/keyphrase_tfidf_vectorizer.py
--rw-r--r--   0 tim        (501) staff       (20)    14700 2022-05-16 14:02:54.000000 keyphrase-vectorizers-0.0.8/keyphrase_vectorizers/keyphrase_vectorizer_mixin.py
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2022-05-16 15:03:08.729515 keyphrase-vectorizers-0.0.8/keyphrase_vectorizers.egg-info/
--rw-r--r--   0 tim        (501) staff       (20)    25357 2022-05-16 15:03:08.000000 keyphrase-vectorizers-0.0.8/keyphrase_vectorizers.egg-info/PKG-INFO
--rw-r--r--   0 tim        (501) staff       (20)      581 2022-05-16 15:03:08.000000 keyphrase-vectorizers-0.0.8/keyphrase_vectorizers.egg-info/SOURCES.txt
--rw-r--r--   0 tim        (501) staff       (20)        1 2022-05-16 15:03:08.000000 keyphrase-vectorizers-0.0.8/keyphrase_vectorizers.egg-info/dependency_links.txt
--rw-r--r--   0 tim        (501) staff       (20)       84 2022-05-16 15:03:08.000000 keyphrase-vectorizers-0.0.8/keyphrase_vectorizers.egg-info/requires.txt
--rw-r--r--   0 tim        (501) staff       (20)       28 2022-05-16 15:03:08.000000 keyphrase-vectorizers-0.0.8/keyphrase_vectorizers.egg-info/top_level.txt
--rw-r--r--   0 tim        (501) staff       (20)      103 2021-12-30 02:50:20.000000 keyphrase-vectorizers-0.0.8/pyproject.toml
--rw-r--r--   0 tim        (501) staff       (20)       83 2022-02-12 14:12:27.000000 keyphrase-vectorizers-0.0.8/requirements.txt
--rw-r--r--   0 tim        (501) staff       (20)       38 2022-05-16 15:03:08.730531 keyphrase-vectorizers-0.0.8/setup.cfg
--rw-r--r--   0 tim        (501) staff       (20)     1601 2022-02-14 16:27:34.000000 keyphrase-vectorizers-0.0.8/setup.py
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2022-05-16 15:03:08.727977 keyphrase-vectorizers-0.0.8/tests/
--rw-r--r--   0 tim        (501) staff       (20)        0 2022-02-13 15:39:04.000000 keyphrase-vectorizers-0.0.8/tests/__init__.py
--rw-r--r--   0 tim        (501) staff       (20)     2470 2022-02-14 12:59:18.000000 keyphrase-vectorizers-0.0.8/tests/test_vectorizers.py
--rw-r--r--   0 tim        (501) staff       (20)     6813 2022-05-16 14:58:09.000000 keyphrase-vectorizers-0.0.8/tests/utils.py
+drwxr-xr-x   0 timschopf   (501) staff       (20)        0 2022-06-18 19:13:00.416650 keyphrase-vectorizers-0.0.9/
+-rw-r--r--   0 timschopf   (501) staff       (20)     1518 2022-01-24 16:04:38.000000 keyphrase-vectorizers-0.0.9/LICENSE
+-rw-r--r--   0 timschopf   (501) staff       (20)    25571 2022-06-18 19:13:00.416410 keyphrase-vectorizers-0.0.9/PKG-INFO
+-rw-r--r--   0 timschopf   (501) staff       (20)    24660 2022-06-18 18:44:07.000000 keyphrase-vectorizers-0.0.9/README.md
+drwxr-xr-x   0 timschopf   (501) staff       (20)        0 2022-06-18 19:13:00.413223 keyphrase-vectorizers-0.0.9/keyphrase_vectorizers/
+-rw-r--r--   0 timschopf   (501) staff       (20)      314 2022-02-01 16:42:11.000000 keyphrase-vectorizers-0.0.9/keyphrase_vectorizers/__init__.py
+-rw-r--r--   0 timschopf   (501) staff       (20)       22 2022-06-18 17:55:31.000000 keyphrase-vectorizers-0.0.9/keyphrase_vectorizers/_version.py
+-rw-r--r--   0 timschopf   (501) staff       (20)    13516 2022-05-16 14:09:11.000000 keyphrase-vectorizers-0.0.9/keyphrase_vectorizers/keyphrase_count_vectorizer.py
+-rw-r--r--   0 timschopf   (501) staff       (20)    11136 2022-05-16 14:08:17.000000 keyphrase-vectorizers-0.0.9/keyphrase_vectorizers/keyphrase_tfidf_vectorizer.py
+-rw-r--r--   0 timschopf   (501) staff       (20)    14485 2022-06-18 19:05:15.000000 keyphrase-vectorizers-0.0.9/keyphrase_vectorizers/keyphrase_vectorizer_mixin.py
+drwxr-xr-x   0 timschopf   (501) staff       (20)        0 2022-06-18 19:13:00.416082 keyphrase-vectorizers-0.0.9/keyphrase_vectorizers.egg-info/
+-rw-r--r--   0 timschopf   (501) staff       (20)    25571 2022-06-18 19:12:59.000000 keyphrase-vectorizers-0.0.9/keyphrase_vectorizers.egg-info/PKG-INFO
+-rw-r--r--   0 timschopf   (501) staff       (20)      581 2022-06-18 19:13:00.000000 keyphrase-vectorizers-0.0.9/keyphrase_vectorizers.egg-info/SOURCES.txt
+-rw-r--r--   0 timschopf   (501) staff       (20)        1 2022-06-18 19:12:59.000000 keyphrase-vectorizers-0.0.9/keyphrase_vectorizers.egg-info/dependency_links.txt
+-rw-r--r--   0 timschopf   (501) staff       (20)       84 2022-06-18 19:13:00.000000 keyphrase-vectorizers-0.0.9/keyphrase_vectorizers.egg-info/requires.txt
+-rw-r--r--   0 timschopf   (501) staff       (20)       28 2022-06-18 19:13:00.000000 keyphrase-vectorizers-0.0.9/keyphrase_vectorizers.egg-info/top_level.txt
+-rw-r--r--   0 timschopf   (501) staff       (20)      103 2021-12-30 02:50:20.000000 keyphrase-vectorizers-0.0.9/pyproject.toml
+-rw-r--r--   0 timschopf   (501) staff       (20)       83 2022-02-12 14:12:27.000000 keyphrase-vectorizers-0.0.9/requirements.txt
+-rw-r--r--   0 timschopf   (501) staff       (20)       38 2022-06-18 19:13:00.416721 keyphrase-vectorizers-0.0.9/setup.cfg
+-rw-r--r--   0 timschopf   (501) staff       (20)     1601 2022-02-14 16:27:34.000000 keyphrase-vectorizers-0.0.9/setup.py
+drwxr-xr-x   0 timschopf   (501) staff       (20)        0 2022-06-18 19:13:00.414563 keyphrase-vectorizers-0.0.9/tests/
+-rw-r--r--   0 timschopf   (501) staff       (20)        0 2022-02-13 15:39:04.000000 keyphrase-vectorizers-0.0.9/tests/__init__.py
+-rw-r--r--   0 timschopf   (501) staff       (20)     2470 2022-02-14 12:59:18.000000 keyphrase-vectorizers-0.0.9/tests/test_vectorizers.py
+-rw-r--r--   0 timschopf   (501) staff       (20)     6814 2022-06-18 18:45:13.000000 keyphrase-vectorizers-0.0.9/tests/utils.py
```

### Comparing `keyphrase-vectorizers-0.0.8/LICENSE` & `keyphrase-vectorizers-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `keyphrase-vectorizers-0.0.8/PKG-INFO` & `keyphrase-vectorizers-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyphrase-vectorizers
-Version: 0.0.8
+Version: 0.0.9
 Summary: Set of vectorizers that extract keyphrases with part-of-speech patterns from a collection of text documents and convert them into a document-keyphrase matrix.
 Home-page: https://github.com/TimSchopf/KeyphraseVectorizers
 Author: Tim Schopf
 Author-email: tim.schopf@t-online.de.de
 License: BSD 3-Clause "New" or "Revised" License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -135,15 +135,15 @@
         in information retrieval."""]
         
 # Init default vectorizer.
 vectorizer = KeyphraseCountVectorizer()
 
 # Print parameters
 print(vectorizer.get_params())
->> > {'binary': False, 'dtype': <class 'numpy.int64'>, 'lowercase': True, 'max_df': None, 'min_df': None, 'pos_pattern': '<J.*>*<N.*>+', 'spacy_pipeline': 'en_core_web_sm', 'stop_words': None, 'workers': 1}
+>>> {'binary': False, 'dtype': <class 'numpy.int64'>, 'lowercase': True, 'max_df': None, 'min_df': None, 'pos_pattern': '<J.*>*<N.*>+', 'spacy_pipeline': 'en_core_web_sm', 'stop_words': None, 'workers': 1}
 ```
 
 By default, the vectorizer is initialized for the English language. That means, an English `spacy_pipeline` is
 specified, no `stop_words` are removed, and the `pos_pattern` extracts keywords that have 0 or more adjectives,
 followed by 1 or more nouns using the English spaCy part-of-speech tags.
 
 ```python
@@ -387,22 +387,23 @@
   ('supervised learning', 0.6779), 
   ('supervised learning algorithm', 0.6992)], 
  [('document content', 0.3988), 
   ('information retrieval environment', 0.5166), 
   ('information retrieval', 0.5792), 
   ('keywords', 0.6046), 
   ('document relevance', 0.633)]]
-
 ```
 
 This allows us to make sure that we do not cut off important words caused by defining our n-gram range too short. For
 example, we would not have found the keyphrase "supervised learning algorithm" with `keyphrase_ngram_range=(1,2)`.
 Furthermore, we avoid to get keyphrases that are slightly off-key like "labeled training", "signal supervised" or
 "keywords quickly".
 
+For more tips on how to use the KeyphraseVectorizers together with KeyBERT, visit [this guide](https://maartengr.github.io/KeyBERT/guides/countvectorizer.html#keyphrasevectorizers "KeyBERT rCountVectorizer Guide").
+
 <a name="#topic-modeling-with-bertopic-and-keyphrasevectorizers"/></a>
 
 ### Topic modeling with [BERTopic](https://github.com/MaartenGr/BERTopic "BERTopic repository") and KeyphraseVectorizers
 
 [Back to Table of Contents](#toc)
 
 Similar to the application with KeyBERT, the keyphrase vectorizers can be used to obtain grammatically correct keyphrases as
```

### Comparing `keyphrase-vectorizers-0.0.8/README.md` & `keyphrase-vectorizers-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         in information retrieval."""]
         
 # Init default vectorizer.
 vectorizer = KeyphraseCountVectorizer()
 
 # Print parameters
 print(vectorizer.get_params())
->> > {'binary': False, 'dtype': <class 'numpy.int64'>, 'lowercase': True, 'max_df': None, 'min_df': None, 'pos_pattern': '<J.*>*<N.*>+', 'spacy_pipeline': 'en_core_web_sm', 'stop_words': None, 'workers': 1}
+>>> {'binary': False, 'dtype': <class 'numpy.int64'>, 'lowercase': True, 'max_df': None, 'min_df': None, 'pos_pattern': '<J.*>*<N.*>+', 'spacy_pipeline': 'en_core_web_sm', 'stop_words': None, 'workers': 1}
 ```
 
 By default, the vectorizer is initialized for the English language. That means, an English `spacy_pipeline` is
 specified, no `stop_words` are removed, and the `pos_pattern` extracts keywords that have 0 or more adjectives,
 followed by 1 or more nouns using the English spaCy part-of-speech tags.
 
 ```python
@@ -367,22 +367,23 @@
   ('supervised learning', 0.6779), 
   ('supervised learning algorithm', 0.6992)], 
  [('document content', 0.3988), 
   ('information retrieval environment', 0.5166), 
   ('information retrieval', 0.5792), 
   ('keywords', 0.6046), 
   ('document relevance', 0.633)]]
-
 ```
 
 This allows us to make sure that we do not cut off important words caused by defining our n-gram range too short. For
 example, we would not have found the keyphrase "supervised learning algorithm" with `keyphrase_ngram_range=(1,2)`.
 Furthermore, we avoid to get keyphrases that are slightly off-key like "labeled training", "signal supervised" or
 "keywords quickly".
 
+For more tips on how to use the KeyphraseVectorizers together with KeyBERT, visit [this guide](https://maartengr.github.io/KeyBERT/guides/countvectorizer.html#keyphrasevectorizers "KeyBERT rCountVectorizer Guide").
+
 <a name="#topic-modeling-with-bertopic-and-keyphrasevectorizers"/></a>
 
 ### Topic modeling with [BERTopic](https://github.com/MaartenGr/BERTopic "BERTopic repository") and KeyphraseVectorizers
 
 [Back to Table of Contents](#toc)
 
 Similar to the application with KeyBERT, the keyphrase vectorizers can be used to obtain grammatically correct keyphrases as
```

### Comparing `keyphrase-vectorizers-0.0.8/keyphrase_vectorizers/keyphrase_count_vectorizer.py` & `keyphrase-vectorizers-0.0.9/keyphrase_vectorizers/keyphrase_count_vectorizer.py`

 * *Files identical despite different names*

### Comparing `keyphrase-vectorizers-0.0.8/keyphrase_vectorizers/keyphrase_tfidf_vectorizer.py` & `keyphrase-vectorizers-0.0.9/keyphrase_vectorizers/keyphrase_tfidf_vectorizer.py`

 * *Files identical despite different names*

### Comparing `keyphrase-vectorizers-0.0.8/keyphrase_vectorizers/keyphrase_vectorizer_mixin.py` & `keyphrase-vectorizers-0.0.9/keyphrase_vectorizers/keyphrase_vectorizer_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -271,16 +271,17 @@
                 logger.setLevel(logging.DEBUG)
                 logger.info(
                     'It looks like you do not have downloaded a list of stopwords yet. It is attempted to download the stopwords now.')
                 nltk.download('stopwords')
                 stop_words_list = set(nltk.corpus.stopwords.words(stop_words))
 
         # add spaCy POS tags for documents
-        spacy_exclude = ['parser', 'ner', 'entity_linker', 'entity_ruler', 'textcat', 'textcat_multilabel',
-                         'lemmatizer', 'morphologizer', 'senter', 'sentencizer', 'transformer']
+
+        # ToDo: add parameter to be able to exclude custom pipeline components for faster processing
+        spacy_exclude = []
         try:
             nlp = spacy.load(spacy_pipeline,
                              exclude=spacy_exclude)
 
         except OSError:
             # set logger
             logger = logging.getLogger('KeyphraseVectorizer')
@@ -292,31 +293,28 @@
             logger.setLevel(logging.DEBUG)
             logger.info(
                 'It looks like the selected spaCy pipeline is not downloaded yet. It is attempted to download the spaCy pipeline now.')
             spacy.cli.download(spacy_pipeline)
             nlp = spacy.load(spacy_pipeline,
                              exclude=spacy_exclude)
 
-        # add rule based sentence boundary detection
-        nlp.add_pipe('sentencizer')
-
         keyphrases_list = []
         if workers != 1:
             os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
         # split large documents in smaller chunks, so that spacy can process them without memory issues
         docs_list = []
         # set maximal character length of documents for spaCy processing
         max_doc_length = 1000000
         for document in document_list:
             if len(document) > max_doc_length:
-                docs_list.append(self._split_long_document(text=document, max_text_length=max_doc_length))
+                docs_list.extend(self._split_long_document(text=document, max_text_length=max_doc_length))
             else:
-                docs_list.append([document])
-        document_list = [text for split_text in docs_list for text in split_text]
+                docs_list.append(document)
+        document_list = docs_list
         del docs_list
 
         # increase max length of documents that spaCy can parse
         # (should only be done if parser and ner are not used due to memory issues)
         nlp.max_length = max([len(doc) for doc in document_list]) + 100
 
         cp = nltk.RegexpParser('CHUNK: {(' + pos_pattern + ')}')
```

### Comparing `keyphrase-vectorizers-0.0.8/keyphrase_vectorizers.egg-info/PKG-INFO` & `keyphrase-vectorizers-0.0.9/keyphrase_vectorizers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyphrase-vectorizers
-Version: 0.0.8
+Version: 0.0.9
 Summary: Set of vectorizers that extract keyphrases with part-of-speech patterns from a collection of text documents and convert them into a document-keyphrase matrix.
 Home-page: https://github.com/TimSchopf/KeyphraseVectorizers
 Author: Tim Schopf
 Author-email: tim.schopf@t-online.de.de
 License: BSD 3-Clause "New" or "Revised" License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -135,15 +135,15 @@
         in information retrieval."""]
         
 # Init default vectorizer.
 vectorizer = KeyphraseCountVectorizer()
 
 # Print parameters
 print(vectorizer.get_params())
->> > {'binary': False, 'dtype': <class 'numpy.int64'>, 'lowercase': True, 'max_df': None, 'min_df': None, 'pos_pattern': '<J.*>*<N.*>+', 'spacy_pipeline': 'en_core_web_sm', 'stop_words': None, 'workers': 1}
+>>> {'binary': False, 'dtype': <class 'numpy.int64'>, 'lowercase': True, 'max_df': None, 'min_df': None, 'pos_pattern': '<J.*>*<N.*>+', 'spacy_pipeline': 'en_core_web_sm', 'stop_words': None, 'workers': 1}
 ```
 
 By default, the vectorizer is initialized for the English language. That means, an English `spacy_pipeline` is
 specified, no `stop_words` are removed, and the `pos_pattern` extracts keywords that have 0 or more adjectives,
 followed by 1 or more nouns using the English spaCy part-of-speech tags.
 
 ```python
@@ -387,22 +387,23 @@
   ('supervised learning', 0.6779), 
   ('supervised learning algorithm', 0.6992)], 
  [('document content', 0.3988), 
   ('information retrieval environment', 0.5166), 
   ('information retrieval', 0.5792), 
   ('keywords', 0.6046), 
   ('document relevance', 0.633)]]
-
 ```
 
 This allows us to make sure that we do not cut off important words caused by defining our n-gram range too short. For
 example, we would not have found the keyphrase "supervised learning algorithm" with `keyphrase_ngram_range=(1,2)`.
 Furthermore, we avoid to get keyphrases that are slightly off-key like "labeled training", "signal supervised" or
 "keywords quickly".
 
+For more tips on how to use the KeyphraseVectorizers together with KeyBERT, visit [this guide](https://maartengr.github.io/KeyBERT/guides/countvectorizer.html#keyphrasevectorizers "KeyBERT rCountVectorizer Guide").
+
 <a name="#topic-modeling-with-bertopic-and-keyphrasevectorizers"/></a>
 
 ### Topic modeling with [BERTopic](https://github.com/MaartenGr/BERTopic "BERTopic repository") and KeyphraseVectorizers
 
 [Back to Table of Contents](#toc)
 
 Similar to the application with KeyBERT, the keyphrase vectorizers can be used to obtain grammatically correct keyphrases as
```

### Comparing `keyphrase-vectorizers-0.0.8/keyphrase_vectorizers.egg-info/SOURCES.txt` & `keyphrase-vectorizers-0.0.9/keyphrase_vectorizers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keyphrase-vectorizers-0.0.8/setup.py` & `keyphrase-vectorizers-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `keyphrase-vectorizers-0.0.8/tests/test_vectorizers.py` & `keyphrase-vectorizers-0.0.9/tests/test_vectorizers.py`

 * *Files identical despite different names*

### Comparing `keyphrase-vectorizers-0.0.8/tests/utils.py` & `keyphrase-vectorizers-0.0.9/tests/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
                                       'inductive bias', 'information retrieval', 'information retrieval environment',
                                       'input', 'input object', 'interest', 'keywords', 'learning', 'learning algorithm',
                                       'list', 'machine', 'main topics', 'new examples', 'optimal scenario', 'output',
                                       'output pairs', 'output value', 'overlap', 'pair', 'phrases', 'precise summary',
                                       'set', 'supervised learning', 'supervisory signal', 'task', 'training data',
                                       'training examples', 'unseen instances', 'unseen situations', 'users',
                                       'various applications', 'vector', 'way']
+
     return sorted_english_test_keyphrases
 
 
 def get_german_test_keyphrases():
     sorted_german_test_keyphrases = ['advokat', 'angesehenen bürgerlichen familie', 'ausbildung', 'bäckers',
                                      'dichtkunst',
                                      'ehefrau elisabetha dorothea schiller', 'frankfurt', 'friedrich schiller',
```

