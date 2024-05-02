# Comparing `tmp/patent_chart-0.2.8.tar.gz` & `tmp/patent_chart-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patent_chart-0.2.8.tar", max compression
+gzip compressed data, was "patent_chart-0.2.9.tar", max compression
```

## Comparing `patent_chart-0.2.8.tar` & `patent_chart-0.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2024-02-02 22:00:15.933827 patent_chart-0.2.8/README.md
--rw-r--r--   0        0        0        0 2024-04-03 22:16:17.760177 patent_chart-0.2.8/patent_chart/__init__.py
--rw-r--r--   0        0        0     3440 2024-02-02 22:00:15.821601 patent_chart-0.2.8/patent_chart/citation.py
--rw-r--r--   0        0        0     1759 2024-04-06 03:36:49.841147 patent_chart-0.2.8/patent_chart/data_structures.py
--rw-r--r--   0        0        0     1843 2024-02-02 22:00:15.871024 patent_chart-0.2.8/patent_chart/embeddings.py
--rw-r--r--   0        0        0     2811 2024-02-02 22:00:15.824681 patent_chart-0.2.8/patent_chart/evaluation.py
--rw-r--r--   0        0        0      498 2024-02-02 22:00:15.823970 patent_chart-0.2.8/patent_chart/filtering.py
--rw-r--r--   0        0        0    37060 2024-04-06 03:36:49.842435 patent_chart-0.2.8/patent_chart/generator.py
--rw-r--r--   0        0        0    11496 2024-04-07 17:08:25.982481 patent_chart-0.2.8/patent_chart/google_patents.py
--rw-r--r--   0        0        0     3838 2024-02-02 22:00:15.872576 patent_chart-0.2.8/patent_chart/integrationtests.py
--rw-r--r--   0        0        0    64508 2024-04-02 04:43:42.390709 patent_chart-0.2.8/patent_chart/parser.py
--rw-r--r--   0        0        0     4536 2024-04-07 17:09:21.646564 patent_chart-0.2.8/patent_chart/pinecone.py
--rw-r--r--   0        0        0     5277 2024-04-06 03:36:49.846114 patent_chart-0.2.8/patent_chart/ranking.py
--rw-r--r--   0        0        0      591 2024-02-02 22:00:15.820971 patent_chart-0.2.8/patent_chart/redis_utils.py
--rw-r--r--   0        0        0     5103 2024-02-02 22:00:15.870154 patent_chart-0.2.8/patent_chart/requests_utils.py
--rw-r--r--   0        0        0     5931 2024-04-06 03:36:49.847015 patent_chart-0.2.8/patent_chart/search_index.py
--rw-r--r--   0        0        0      567 2024-02-20 15:54:25.646442 patent_chart-0.2.8/patent_chart/settings.py
--rw-r--r--   0        0        0    31579 2024-04-02 04:43:42.392082 patent_chart-0.2.8/patent_chart/tests.py
--rw-r--r--   0        0        0     6106 2024-04-06 03:51:00.343412 patent_chart-0.2.8/patent_chart/uspto_parse.py
--rw-r--r--   0        0        0     1825 2024-02-02 22:00:15.871782 patent_chart-0.2.8/patent_chart/utils.py
--rw-r--r--   0        0        0     1082 2024-04-07 17:22:09.343062 patent_chart-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 patent_chart-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-02 22:00:15.933827 patent_chart-0.2.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 22:16:17.760177 patent_chart-0.2.9/patent_chart/__init__.py
+-rw-r--r--   0        0        0     3440 2024-02-02 22:00:15.821601 patent_chart-0.2.9/patent_chart/citation.py
+-rw-r--r--   0        0        0     1835 2024-04-12 04:09:15.526893 patent_chart-0.2.9/patent_chart/data_structures.py
+-rw-r--r--   0        0        0     1843 2024-02-02 22:00:15.871024 patent_chart-0.2.9/patent_chart/embeddings.py
+-rw-r--r--   0        0        0     2811 2024-02-02 22:00:15.824681 patent_chart-0.2.9/patent_chart/evaluation.py
+-rw-r--r--   0        0        0      498 2024-02-02 22:00:15.823970 patent_chart-0.2.9/patent_chart/filtering.py
+-rw-r--r--   0        0        0    37060 2024-04-08 15:49:45.142667 patent_chart-0.2.9/patent_chart/generator.py
+-rw-r--r--   0        0        0    11930 2024-04-12 04:10:48.138187 patent_chart-0.2.9/patent_chart/google_patents.py
+-rw-r--r--   0        0        0     3838 2024-02-02 22:00:15.872576 patent_chart-0.2.9/patent_chart/integrationtests.py
+-rw-r--r--   0        0        0    64508 2024-04-02 04:43:42.390709 patent_chart-0.2.9/patent_chart/parser.py
+-rw-r--r--   0        0        0     4536 2024-04-08 17:03:44.566485 patent_chart-0.2.9/patent_chart/pinecone.py
+-rw-r--r--   0        0        0     5277 2024-04-08 15:49:45.145419 patent_chart-0.2.9/patent_chart/ranking.py
+-rw-r--r--   0        0        0      591 2024-02-02 22:00:15.820971 patent_chart-0.2.9/patent_chart/redis_utils.py
+-rw-r--r--   0        0        0     5103 2024-02-02 22:00:15.870154 patent_chart-0.2.9/patent_chart/requests_utils.py
+-rw-r--r--   0        0        0     5931 2024-04-08 15:49:45.146741 patent_chart-0.2.9/patent_chart/search_index.py
+-rw-r--r--   0        0        0      567 2024-02-20 15:54:25.646442 patent_chart-0.2.9/patent_chart/settings.py
+-rw-r--r--   0        0        0    31579 2024-04-02 04:43:42.392082 patent_chart-0.2.9/patent_chart/tests.py
+-rw-r--r--   0        0        0     6106 2024-04-08 15:49:45.147802 patent_chart-0.2.9/patent_chart/uspto_parse.py
+-rw-r--r--   0        0        0     1825 2024-02-02 22:00:15.871782 patent_chart-0.2.9/patent_chart/utils.py
+-rw-r--r--   0        0        0     1082 2024-04-12 04:11:13.978429 patent_chart-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 patent_chart-0.2.9/PKG-INFO
```

### Comparing `patent_chart-0.2.8/patent_chart/citation.py` & `patent_chart-0.2.9/patent_chart/citation.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.8/patent_chart/data_structures.py` & `patent_chart-0.2.9/patent_chart/data_structures.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,8 +52,12 @@
     unique_id: PatentUniqueID
     specification: Optional[str] = None
     claims: Optional[str] = None
     title: Optional[str] = None
     text: Optional[str] = None
     text_format: Optional[str] = None
     filing_date: Optional[str] = None
-    priority_date: Optional[str] = None
+    priority_date: Optional[str] = None
+
+    @classmethod
+    def from_json(cls, json):
+        return cls(**json)
```

### Comparing `patent_chart-0.2.8/patent_chart/embeddings.py` & `patent_chart-0.2.9/patent_chart/embeddings.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.8/patent_chart/evaluation.py` & `patent_chart-0.2.9/patent_chart/evaluation.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.8/patent_chart/generator.py` & `patent_chart-0.2.9/patent_chart/generator.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.8/patent_chart/google_patents.py` & `patent_chart-0.2.9/patent_chart/google_patents.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 import pathlib
 import time
 import typing
+import logging
 import re
 import xml.etree.ElementTree as ET
 from datetime import datetime
 from functools import cached_property
 from logging import getLogger
 
 from langchain.text_splitter import RecursiveCharacterTextSplitter
@@ -60,15 +61,16 @@
 filing_date_regex = re.compile(r'filing|filed')
 
 
 class GooglePatent:
     def __init__(self, patent_id, html_text=None) -> None:
         self.patent_id = patent_id
         if html_text is None:
-            self.soup = BeautifulSoup(requests.get(f"https://us-west1-careful-ai.cloudfunctions.net/google-patents?patent_id={patent_id}").text, 'html.parser')
+            url = f"https://us-west1-careful-ai.cloudfunctions.net/google-patents?patent_number={patent_id}&view_source=false"
+            self.soup = BeautifulSoup(requests.get(url).text, 'html.parser')
         else:
             self.soup = BeautifulSoup(html_text, 'html.parser')
     
     @classmethod
     def from_html_text(cls, patent_id, html_text):
         return cls(patent_id, html_text)
 
@@ -182,27 +184,35 @@
         header = self.soup.find('h3', id='patentCitations')
         table = header.find_next_sibling()
         return [a.text for a in table.find_all('a')]
 
 
 def parse_google_patent(patent_unique_id: PatentUniqueID) ->  GoogleParsedPatent | None:
     # Uses selenium to get dates -- probably faster way but whatever
-    patent = GooglePatent(patent_unique_id)
+    patent = GooglePatent(str(patent_unique_id))
 
-    return GoogleParsedPatent(
+    google_parsed_patent = GoogleParsedPatent(
         unique_id=patent_unique_id,
         specification=patent.specification_text,
         claims=patent.claims_text,
         title=patent.title,
         text=str(patent.soup),
         text_format='google_html_with_selenium',
-        filing_date=patent.filing_date.strftime('%Y-%m-%d'),
-        priority_date=patent.inferred_priority_date.strftime('%Y-%m-%d'),
+        filing_date=patent.filing_date.strftime('%Y-%m-%d') if patent.filing_date else None,
+        priority_date=patent.inferred_priority_date.strftime('%Y-%m-%d') if patent.inferred_priority_date else None,
     )
 
+    if patent.filing_date:
+        google_parsed_patent.filing_date = patent.filing_date.strftime('%Y-%m-%d')
+
+    if patent.inferred_priority_date:
+        google_parsed_patent.priority_date = patent.inferred_priority_date.strftime('%Y-%m-%d')
+
+    return google_parsed_patent
+
 
 def extract_text_recursive(element: ET.Element):
     text = ''
     if element.text:
         text += element.text
     for child in element:
         text += extract_text_recursive(child)
```

### Comparing `patent_chart-0.2.8/patent_chart/integrationtests.py` & `patent_chart-0.2.9/patent_chart/integrationtests.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.8/patent_chart/parser.py` & `patent_chart-0.2.9/patent_chart/parser.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.8/patent_chart/pinecone.py` & `patent_chart-0.2.9/patent_chart/pinecone.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.8/patent_chart/ranking.py` & `patent_chart-0.2.9/patent_chart/ranking.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.8/patent_chart/redis_utils.py` & `patent_chart-0.2.9/patent_chart/redis_utils.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.8/patent_chart/requests_utils.py` & `patent_chart-0.2.9/patent_chart/requests_utils.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.8/patent_chart/search_index.py` & `patent_chart-0.2.9/patent_chart/search_index.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.8/patent_chart/settings.py` & `patent_chart-0.2.9/patent_chart/settings.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.8/patent_chart/tests.py` & `patent_chart-0.2.9/patent_chart/tests.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.8/patent_chart/uspto_parse.py` & `patent_chart-0.2.9/patent_chart/uspto_parse.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.8/patent_chart/utils.py` & `patent_chart-0.2.9/patent_chart/utils.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.8/pyproject.toml` & `patent_chart-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "patent-chart"
-version = "0.2.8"
+version = "0.2.9"
 description = "Automated invalidity contention charts"
 authors = ["Josh Hedtke"]
 license = "Proprietary"
 readme = "README.md"
 
 exclude = ["experiments.ipynb"]
```

### Comparing `patent_chart-0.2.8/PKG-INFO` & `patent_chart-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patent-chart
-Version: 0.2.8
+Version: 0.2.9
 Summary: Automated invalidity contention charts
 License: Proprietary
 Author: Josh Hedtke
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

