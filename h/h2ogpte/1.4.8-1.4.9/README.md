# Comparing `tmp/h2ogpte-1.4.8-py3-none-any.whl.zip` & `tmp/h2ogpte-1.4.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 45581 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1520 b- defN 24-Mar-22 16:42 h2ogpte/__init__.py
--rw-r--r--  2.0 unx     1152 b- defN 24-Feb-07 17:38 h2ogpte/errors.py
--rw-r--r--  2.0 unx    91412 b- defN 24-Mar-22 16:42 h2ogpte/h2ogpte.py
--rw-r--r--  2.0 unx    91607 b- defN 24-Mar-22 16:42 h2ogpte/h2ogpte_async.py
--rw-r--r--  2.0 unx    15673 b- defN 24-Mar-20 16:21 h2ogpte/session.py
--rw-r--r--  2.0 unx    15181 b- defN 24-Mar-20 16:21 h2ogpte/session_async.py
--rw-r--r--  2.0 unx     8515 b- defN 24-Mar-20 16:21 h2ogpte/types.py
--rw-r--r--  2.0 unx     3715 b- defN 24-Mar-22 18:05 h2ogpte-1.4.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-22 18:05 h2ogpte-1.4.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Mar-22 18:05 h2ogpte-1.4.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      836 b- defN 24-Mar-22 18:05 h2ogpte-1.4.8.dist-info/RECORD
-11 files, 229711 bytes uncompressed, 44195 bytes compressed:  80.8%
+Zip file size: 45580 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1520 b- defN 24-Mar-22 20:19 h2ogpte/__init__.py
+-rw-r--r--  2.0 unx     1152 b- defN 24-Mar-11 17:35 h2ogpte/errors.py
+-rw-r--r--  2.0 unx    91412 b- defN 24-Mar-22 18:15 h2ogpte/h2ogpte.py
+-rw-r--r--  2.0 unx    91607 b- defN 24-Mar-22 18:15 h2ogpte/h2ogpte_async.py
+-rw-r--r--  2.0 unx    15673 b- defN 24-Mar-20 01:21 h2ogpte/session.py
+-rw-r--r--  2.0 unx    15181 b- defN 24-Mar-20 01:21 h2ogpte/session_async.py
+-rw-r--r--  2.0 unx     8515 b- defN 24-Mar-20 16:04 h2ogpte/types.py
+-rw-r--r--  2.0 unx     3715 b- defN 24-Mar-22 21:41 h2ogpte-1.4.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-22 21:41 h2ogpte-1.4.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Mar-22 21:41 h2ogpte-1.4.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      836 b- defN 24-Mar-22 21:41 h2ogpte-1.4.9.dist-info/RECORD
+11 files, 229711 bytes uncompressed, 44194 bytes compressed:  80.8%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: h2ogpte/session_async.py
 Comment: 
 
 Filename: h2ogpte/types.py
 Comment: 
 
-Filename: h2ogpte-1.4.8.dist-info/METADATA
+Filename: h2ogpte-1.4.9.dist-info/METADATA
 Comment: 
 
-Filename: h2ogpte-1.4.8.dist-info/WHEEL
+Filename: h2ogpte-1.4.9.dist-info/WHEEL
 Comment: 
 
-Filename: h2ogpte-1.4.8.dist-info/top_level.txt
+Filename: h2ogpte-1.4.9.dist-info/top_level.txt
 Comment: 
 
-Filename: h2ogpte-1.4.8.dist-info/RECORD
+Filename: h2ogpte-1.4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## h2ogpte/__init__.py

```diff
@@ -1,13 +1,13 @@
 from h2ogpte.session import Session
 from h2ogpte.h2ogpte import H2OGPTE
 from h2ogpte.h2ogpte_async import H2OGPTEAsync
 from h2ogpte.session_async import SessionAsync
 
-__version__ = "1.4.8"
+__version__ = "1.4.9"
 
 __all__ = [
     "H2OGPTE",
     "H2OGPTEAsync",
     "Session",
     "SessionAsync",
 ]
```

## Comparing `h2ogpte-1.4.8.dist-info/METADATA` & `h2ogpte-1.4.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h2ogpte
-Version: 1.4.8
+Version: 1.4.9
 Summary: Client library for Enterprise h2oGPTe
 Author-email: "H2O.ai, Inc." <support@h2o.ai>
 Project-URL: Source, https://github.com/h2oai/h2ogpte
 Project-URL: Issues, https://github.com/h2oai/h2ogpte/issues
 Project-URL: Documentation, https://h2oai.github.io/h2ogpte/
 Keywords: information-retrieval,LLM,large-language-models,question-answering,search,semantic-search,analytical-search,lexical-search,document-search,natural-language-querying
 Classifier: Development Status :: 4 - Beta
```

