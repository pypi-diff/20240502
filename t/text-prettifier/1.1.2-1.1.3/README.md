# Comparing `tmp/text_prettifier-1.1.2.tar.gz` & `tmp/text_prettifier-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_prettifier-1.1.2.tar", last modified: Thu May  2 16:24:42 2024, max compression
+gzip compressed data, was "text_prettifier-1.1.3.tar", last modified: Thu May  2 17:23:54 2024, max compression
```

## Comparing `text_prettifier-1.1.2.tar` & `text_prettifier-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:24:42.921746 text_prettifier-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-02 16:24:39.000000 text_prettifier-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-02 16:24:42.921746 text_prettifier-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-02 16:24:39.000000 text_prettifier-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:24:42.921746 text_prettifier-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-02 16:24:39.000000 text_prettifier-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:24:42.921746 text_prettifier-1.1.2/text_prettifier/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-02 16:24:39.000000 text_prettifier-1.1.2/text_prettifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-02 16:24:39.000000 text_prettifier-1.1.2/text_prettifier/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7705 2024-05-02 16:24:39.000000 text_prettifier-1.1.2/text_prettifier/text_prettifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-02 16:24:39.000000 text_prettifier-1.1.2/text_prettifier/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:24:42.921746 text_prettifier-1.1.2/text_prettifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-02 16:24:42.000000 text_prettifier-1.1.2/text_prettifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-02 16:24:42.000000 text_prettifier-1.1.2/text_prettifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:24:42.000000 text_prettifier-1.1.2/text_prettifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 16:24:42.000000 text_prettifier-1.1.2/text_prettifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 16:24:42.000000 text_prettifier-1.1.2/text_prettifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:23:54.173380 text_prettifier-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-02 17:23:50.000000 text_prettifier-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-02 17:23:54.173380 text_prettifier-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-02 17:23:50.000000 text_prettifier-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 17:23:54.173380 text_prettifier-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-02 17:23:50.000000 text_prettifier-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:23:54.173380 text_prettifier-1.1.3/text_prettifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-02 17:23:50.000000 text_prettifier-1.1.3/text_prettifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-02 17:23:50.000000 text_prettifier-1.1.3/text_prettifier/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7705 2024-05-02 17:23:50.000000 text_prettifier-1.1.3/text_prettifier/text_prettifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-02 17:23:50.000000 text_prettifier-1.1.3/text_prettifier/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:23:54.173380 text_prettifier-1.1.3/text_prettifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-02 17:23:54.000000 text_prettifier-1.1.3/text_prettifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-02 17:23:54.000000 text_prettifier-1.1.3/text_prettifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:23:54.000000 text_prettifier-1.1.3/text_prettifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 17:23:54.000000 text_prettifier-1.1.3/text_prettifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 17:23:54.000000 text_prettifier-1.1.3/text_prettifier.egg-info/top_level.txt
```

### Comparing `text_prettifier-1.1.2/LICENSE` & `text_prettifier-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `text_prettifier-1.1.2/PKG-INFO` & `text_prettifier-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-prettifier
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python library for cleaning and preprocessing text data by removing,emojies,internet words, special characters, digits, HTML tags, URLs, and stopwords.
 Author: Qadeer Ahmad
 Author-email: mrqadeer1231122@gmail.com
 Keywords: text cleaning,text preprocessing,text scrubber,NLP,natural language processing,data cleaning,data preprocessing,string manipulation,text manipulation,stopwords removal,contractions expansion,text normalization,text sanitization,internet words removal,emojis removal,emojis killer
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `text_prettifier-1.1.2/README.md` & `text_prettifier-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `text_prettifier-1.1.2/setup.py` & `text_prettifier-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.2'
+VERSION = '1.1.3'  
 DESCRIPTION = "A Python library for cleaning and preprocessing text data by removing,emojies,internet words, special characters, digits, HTML tags, URLs, and stopwords."
 
 
 KEYWORDS = [
     'text cleaning', 'text preprocessing', 'text scrubber', 'NLP', 'natural language processing',
     'data cleaning', 'data preprocessing', 'string manipulation', 'text manipulation',
     'stopwords removal', 'contractions expansion', 'text normalization', 'text sanitization',
```

### Comparing `text_prettifier-1.1.2/text_prettifier/text_prettifier.py` & `text_prettifier-1.1.3/text_prettifier/text_prettifier.py`

 * *Files identical despite different names*

### Comparing `text_prettifier-1.1.2/text_prettifier.egg-info/PKG-INFO` & `text_prettifier-1.1.3/text_prettifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-prettifier
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python library for cleaning and preprocessing text data by removing,emojies,internet words, special characters, digits, HTML tags, URLs, and stopwords.
 Author: Qadeer Ahmad
 Author-email: mrqadeer1231122@gmail.com
 Keywords: text cleaning,text preprocessing,text scrubber,NLP,natural language processing,data cleaning,data preprocessing,string manipulation,text manipulation,stopwords removal,contractions expansion,text normalization,text sanitization,internet words removal,emojis removal,emojis killer
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

