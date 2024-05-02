# Comparing `tmp/pybangla-0.0.4.tar.gz` & `tmp/pybangla-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybangla-0.0.4.tar", last modified: Wed May  1 18:21:50 2024, max compression
+gzip compressed data, was "pybangla-1.0.0.tar", last modified: Wed May  1 20:03:03 2024, max compression
```

## Comparing `pybangla-0.0.4.tar` & `pybangla-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:21:50.770495 pybangla-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:21:42.000000 pybangla-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14128 2024-05-01 18:21:50.770495 pybangla-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13570 2024-05-01 18:21:42.000000 pybangla-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:21:50.766495 pybangla-0.0.4/pybangla/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-01 18:21:42.000000 pybangla-0.0.4/pybangla/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:21:50.770495 pybangla-0.0.4/pybangla/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:21:42.000000 pybangla-0.0.4/pybangla/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-05-01 18:21:42.000000 pybangla-0.0.4/pybangla/module/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-05-01 18:21:42.000000 pybangla-0.0.4/pybangla/module/date_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-05-01 18:21:42.000000 pybangla-0.0.4/pybangla/module/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    16398 2024-05-01 18:21:42.000000 pybangla-0.0.4/pybangla/module/number_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    15187 2024-05-01 18:21:42.000000 pybangla-0.0.4/pybangla/module/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-01 18:21:42.000000 pybangla-0.0.4/pybangla/module/word_to_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     8917 2024-05-01 18:21:42.000000 pybangla-0.0.4/pybangla/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:21:50.770495 pybangla-0.0.4/pybangla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14128 2024-05-01 18:21:50.000000 pybangla-0.0.4/pybangla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-01 18:21:50.000000 pybangla-0.0.4/pybangla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:21:50.000000 pybangla-0.0.4/pybangla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 18:21:50.000000 pybangla-0.0.4/pybangla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 18:21:50.000000 pybangla-0.0.4/pybangla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:21:50.770495 pybangla-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-01 18:21:42.000000 pybangla-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:21:50.770495 pybangla-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-01 18:21:42.000000 pybangla-0.0.4/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:03:03.349589 pybangla-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:02:58.000000 pybangla-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15743 2024-05-01 20:03:03.349589 pybangla-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-01 20:02:58.000000 pybangla-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:03:03.345589 pybangla-1.0.0/pybangla/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-01 20:02:58.000000 pybangla-1.0.0/pybangla/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:03:03.349589 pybangla-1.0.0/pybangla/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:02:58.000000 pybangla-1.0.0/pybangla/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-05-01 20:02:58.000000 pybangla-1.0.0/pybangla/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-05-01 20:02:58.000000 pybangla-1.0.0/pybangla/module/date_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-01 20:02:58.000000 pybangla-1.0.0/pybangla/module/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-05-01 20:02:58.000000 pybangla-1.0.0/pybangla/module/number_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17929 2024-05-01 20:02:58.000000 pybangla-1.0.0/pybangla/module/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-01 20:02:58.000000 pybangla-1.0.0/pybangla/module/word_to_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-05-01 20:02:58.000000 pybangla-1.0.0/pybangla/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:03:03.349589 pybangla-1.0.0/pybangla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15743 2024-05-01 20:03:03.000000 pybangla-1.0.0/pybangla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-01 20:03:03.000000 pybangla-1.0.0/pybangla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:03:03.000000 pybangla-1.0.0/pybangla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 20:03:03.000000 pybangla-1.0.0/pybangla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 20:03:03.000000 pybangla-1.0.0/pybangla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 20:03:03.349589 pybangla-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-01 20:02:58.000000 pybangla-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:03:03.349589 pybangla-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-01 20:02:58.000000 pybangla-1.0.0/tests/test.py
```

### Comparing `pybangla-0.0.4/PKG-INFO` & `pybangla-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 0.0.4
+Version: 1.0.0
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: DateTime
 Requires-Dist: num2words
 
 
-PYBANGLA is a python3 package for Bengala Number, DateTime and Text Normalizer. This package can be used Normalize the text number and date (ex: number to text vice versa). This framework  also can be used Django, Flask, FastAPI, and others. PYBANGLA module supported operating system Linux/Unix, Mac OS and Windows.
+PYBANGLA is a python3 package for Bangla Number, DateTime and Text Normalizer and Date Extraction. This package can be used Normalize the text number and date (ex: number to text vice versa). This framework  also can be used Django, Flask, FastAPI, and others. PYBANGLA module supported operating system Linux/Unix, Mac OS and Windows.
 Available Features
 
 Features available in PYBANGLA:
 
 1. Text Normalization
 2. Number Conversion
 3. Date Format
@@ -31,16 +31,14 @@
 The easiest way to install pybangla is to use pip:
 
 ```
 pip install pybangla
 ```
 
 
-
-
 # Usage
 
 ## 1. Text Normalization
 ### It supports converting Bangla abbreviations, symbols, and currencies to Bangla textual format.
 
 ```py
 import pybangla
@@ -70,14 +68,24 @@
 text = "আজকের তাপমাত্রা ৪৪°"
 
 #output:
 'আজকের তাপমাত্রা চুয়াল্লিশ ডিগ্রী'
 
 ```
 
+```py
+
+text = "সম্মেলনটি সেপ্টেম্বর ০৫ ২০২৩ তারিখে নির্ধারিত করা হয়েছে. এপ্রিল ২০২৩"
+text = nrml.text_normalizer(text)
+#output:
+
+সম্মেলনটি পাঁচ সেপ্টেম্বর দুই হাজার তেইশ তারিখে নির্ধারিত করা হয়েছে. এক এপ্রিল দুই হাজার তেইশ
+
+```
+
 Supported
 
 ```
 #abbreviations:
 ("সাঃ", "সাল্লাল্লাহু আলাইহি ওয়া সাল্লাম"),                  
 ("আঃ", "আলাইহিস সালাম"),
 ("রাঃ", "রাদিআল্লাহু আনহু"),
@@ -284,34 +292,54 @@
 {'date': '০৪', 'month': 'জানুয়ারি', 'year': '২০২৩', 'weekday': 'বুধবার', 'ls_month': 'বৈশাখ', 'seasons': 'গ্রীষ্ম'}
 
 or
 English:
 
 {'date': '04', 'month': 'January', 'year': '2023', 'weekday': 'Wednesday', 'ls_month': 'Jan', 'seasons': 'Summer'}
 ```
-```
+```py
 import pybangla
 nrml = pybangla.Normalizer()
 
 date = dt.date_format("01-Apr/2023", language="bn")
 print(f"{date}")
 # Output: 
 {'date': '০১', 'month': 'এপ্রিল', 'year': '২০২৩', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
 ```
 
-```
+```py
 import pybangla
 nrml = pybangla.Normalizer()
 en_date = dt.date_format("01-Apr/2023", language="en")
 print(f"{en_date}")
 
 # Output :
 {'date': '01', 'month': 'April', 'year': '2023', 'weekday': 'Saturday', 'ls_month': 'Apr', 'seasons': 'Wet season'}
 ```
 
+## Date extraction
+
+```py
+Rule based Date Extraction
+import pybangla
+nrml = pybangla.Normalizer()
+
+text = "সম্মেলনটি সেপ্টেম্বর ০৫ ২০২৩ তারিখে নির্ধারিত করা হয়েছে. এপ্রিল ২০২৩"
+dates = nrml.date_extraction(text)
+
+#output:
+
+[
+{'date': '০৫', 'month': 'সেপ্টেম্বর', 'year': '২০২৩', 'txt_date': 'পাঁচ', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'মঙ্গলবার', 'ls_month': 'পৌষ', 'seasons': 'শীত'}, 
+
+{'date': '১', 'month': 'এপ্রিল', 'year': '২০২৩', 'txt_date': 'এক', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
+]
+
+```
+
 ## 4. Today, Months, Weekdays, Seasons
 ### It converts Bangla (today, months, weekdays, and seasons) to English and English to Bangla, and vice versa, in a pair format.
 
 ## 1. Today:
 
 ```py
 import pybangla
@@ -469,15 +497,23 @@
 ```
 # Next Upcomming Features
 
 1. Date extraction from normal text sentence and convert it numerical to word(vice versa)
 2. Bangla lemmatization and stemming algorithm
 3. Bangla Tokenizer
 
-# Contribute
-
-If you face any problem feel free to open issue.
 
 # Contact
 If you have any suggestion: Email: saifulbrur79@gmail.com
 
+# Contributor
+
+```
+@misc{BanglaASR ,
+  title={PYBANGLA module use for normalize textual format like text to number and number to text},
+  author={Md Saiful Islam, Hassan Ali Emon,  HM-badhon, Sagor Sarker},
+  howpublished={},
+  year={2024}
+}
+```
+If you face any problem feel free to open issue.
```

### Comparing `pybangla-0.0.4/README.md` & `pybangla-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-PYBANGLA is a python3 package for Bengala Number, DateTime and Text Normalizer. This package can be used Normalize the text number and date (ex: number to text vice versa). This framework  also can be used Django, Flask, FastAPI, and others. PYBANGLA module supported operating system Linux/Unix, Mac OS and Windows.
+PYBANGLA is a python3 package for Bangla Number, DateTime and Text Normalizer and Date Extraction. This package can be used Normalize the text number and date (ex: number to text vice versa). This framework  also can be used Django, Flask, FastAPI, and others. PYBANGLA module supported operating system Linux/Unix, Mac OS and Windows.
 Available Features
 
 Features available in PYBANGLA:
 
 1. Text Normalization
 2. Number Conversion
 3. Date Format
@@ -15,16 +15,14 @@
 The easiest way to install pybangla is to use pip:
 
 ```
 pip install pybangla
 ```
 
 
-
-
 # Usage
 
 ## 1. Text Normalization
 ### It supports converting Bangla abbreviations, symbols, and currencies to Bangla textual format.
 
 ```py
 import pybangla
@@ -54,14 +52,24 @@
 text = "আজকের তাপমাত্রা ৪৪°"
 
 #output:
 'আজকের তাপমাত্রা চুয়াল্লিশ ডিগ্রী'
 
 ```
 
+```py
+
+text = "সম্মেলনটি সেপ্টেম্বর ০৫ ২০২৩ তারিখে নির্ধারিত করা হয়েছে. এপ্রিল ২০২৩"
+text = nrml.text_normalizer(text)
+#output:
+
+সম্মেলনটি পাঁচ সেপ্টেম্বর দুই হাজার তেইশ তারিখে নির্ধারিত করা হয়েছে. এক এপ্রিল দুই হাজার তেইশ
+
+```
+
 Supported
 
 ```
 #abbreviations:
 ("সাঃ", "সাল্লাল্লাহু আলাইহি ওয়া সাল্লাম"),                  
 ("আঃ", "আলাইহিস সালাম"),
 ("রাঃ", "রাদিআল্লাহু আনহু"),
@@ -268,34 +276,54 @@
 {'date': '০৪', 'month': 'জানুয়ারি', 'year': '২০২৩', 'weekday': 'বুধবার', 'ls_month': 'বৈশাখ', 'seasons': 'গ্রীষ্ম'}
 
 or
 English:
 
 {'date': '04', 'month': 'January', 'year': '2023', 'weekday': 'Wednesday', 'ls_month': 'Jan', 'seasons': 'Summer'}
 ```
-```
+```py
 import pybangla
 nrml = pybangla.Normalizer()
 
 date = dt.date_format("01-Apr/2023", language="bn")
 print(f"{date}")
 # Output: 
 {'date': '০১', 'month': 'এপ্রিল', 'year': '২০২৩', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
 ```
 
-```
+```py
 import pybangla
 nrml = pybangla.Normalizer()
 en_date = dt.date_format("01-Apr/2023", language="en")
 print(f"{en_date}")
 
 # Output :
 {'date': '01', 'month': 'April', 'year': '2023', 'weekday': 'Saturday', 'ls_month': 'Apr', 'seasons': 'Wet season'}
 ```
 
+## Date extraction
+
+```py
+Rule based Date Extraction
+import pybangla
+nrml = pybangla.Normalizer()
+
+text = "সম্মেলনটি সেপ্টেম্বর ০৫ ২০২৩ তারিখে নির্ধারিত করা হয়েছে. এপ্রিল ২০২৩"
+dates = nrml.date_extraction(text)
+
+#output:
+
+[
+{'date': '০৫', 'month': 'সেপ্টেম্বর', 'year': '২০২৩', 'txt_date': 'পাঁচ', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'মঙ্গলবার', 'ls_month': 'পৌষ', 'seasons': 'শীত'}, 
+
+{'date': '১', 'month': 'এপ্রিল', 'year': '২০২৩', 'txt_date': 'এক', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
+]
+
+```
+
 ## 4. Today, Months, Weekdays, Seasons
 ### It converts Bangla (today, months, weekdays, and seasons) to English and English to Bangla, and vice versa, in a pair format.
 
 ## 1. Today:
 
 ```py
 import pybangla
@@ -453,15 +481,23 @@
 ```
 # Next Upcomming Features
 
 1. Date extraction from normal text sentence and convert it numerical to word(vice versa)
 2. Bangla lemmatization and stemming algorithm
 3. Bangla Tokenizer
 
-# Contribute
-
-If you face any problem feel free to open issue.
 
 # Contact
 If you have any suggestion: Email: saifulbrur79@gmail.com
 
+# Contributor
+
+```
+@misc{BanglaASR ,
+  title={PYBANGLA module use for normalize textual format like text to number and number to text},
+  author={Md Saiful Islam, Hassan Ali Emon,  HM-badhon, Sagor Sarker},
+  howpublished={},
+  year={2024}
+}
+```
+If you face any problem feel free to open issue.
```

### Comparing `pybangla-0.0.4/pybangla/module/config.py` & `pybangla-1.0.0/pybangla/module/config.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.4/pybangla/module/date_extractor.py` & `pybangla-1.0.0/pybangla/module/date_extractor.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.4/pybangla/module/main.py` & `pybangla-1.0.0/pybangla/module/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 
 import re
 import time
 import datetime
 from .config import Config as cfg
 from .parser import DateParser, TextParser, NumberParser
 from .number_parser import Word2NumberMap
+from .date_extractor import DateExtractor
 dp, tp, npr, wnmp = DateParser(), TextParser(), NumberParser(), Word2NumberMap()
+dt = DateExtractor()
 data = cfg.data
 
 class Normalizer:
     def __init__(self):
 
         self.bn_regex = cfg.bn_regex
     
@@ -105,40 +107,16 @@
         Arg:
             data_{str or list} :  date may string or list of list like ["dd", "mm", "yyyy"]
             language{str}      : specific language format, support bangla and english
 
         return : 
                 Dictonary :  {"date":day, "month": month[0], "year": year, "weekday" : weekday, "ls_month": month[1], "seasons" : month[2]}       
         """
-        if isinstance(date_, list):
-            if len(date_):
-                formatted_date = date_
-        else:
-            split_date = dp.data_splitter(date_)
-            split_date = [i for i in split_date if i]
-
-            if len(split_date) == 1:
-                formatted_date = dp.format_non_punctuation(split_date)
-            else:
-                formatted_date = dp.get_date_indexes(split_date)
-
-        if formatted_date[0] == None and formatted_date[1] == None and formatted_date[2] == None:
-            current_date_object = datetime.date.today()
-            formatted_date = [current_date_object.day, current_date_object.month, current_date_object.year]
-
-        weekday = npr.get_weekday(formatted_date, language)
-        day   = npr._digit_converter(str(formatted_date[0]), language)
-        month = npr.search_month(str(formatted_date[1]), language)
-        year  =  npr._digit_converter(str(formatted_date[2]), language)
-
-        txt_date = npr.number_to_words(day)
-        txt_year = npr.year_in_number(year, language=language)
-
-
-        return {"date":day, "month": month[0], "year": year, "txt_date":txt_date, "txt_year": txt_year, "weekday" : weekday, "ls_month": month[1], "seasons" : month[2]}
+        formated_date = dp.date_processing(date_, language=language)
+        return formated_date
 
     def number_convert(self, number, language="bn"):
         """
         Convert the number digits English -> Bangla  or Bangla -> English
 
         Arg:
             number{str}  :  number string
@@ -164,14 +142,22 @@
         text = tp.processing(text)
         return text
     
     def word2number(self, text):
         text = wnmp.convert_word2number(text)
         return text
     
+    def date_extraction(self, text):
+
+        dates = dt.get_dates(text)
+        formated_date = [self.date_format(i)for i in dates]
+        # print(f"Input: {sentence}: Output: {dates}")
+        return formated_date
+
+    
 if __name__ == "__main__":
 
 
     # Testing Date format
     date_list = [
         "০১-এপ্রিল/২০২৩",
         "১ এপ্রিল ২০২৩"
```

### Comparing `pybangla-0.0.4/pybangla/module/number_parser.py` & `pybangla-1.0.0/pybangla/module/number_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,28 +149,28 @@
                 if i == len(input_list) - 1 or not input_list[i + 1].isdigit():
                     output_list.append(temp), output_status.append(True)
                     temp = []
             else:
                 output_list.append([value]), output_status.append(False)  
         return output_list, output_status
 
-    def find_word_index(self, text:str, word:str)->list:
-        """
-        Word spanning position
-        """
-        start  = text.find(word)
-        end = start+len(word)
-        return [start, end]
-
-    def replace_text_at_position(self, text:str, replacement:str, start_pos:int, end_pos:int)->str:
-        """
-        Replance text using text position
+    # def find_word_index(self, text:str, word:str)->list:
+    #     """
+    #     Word spanning position
+    #     """
+    #     start  = text.find(word)
+    #     end = start+len(word)
+    #     return [start, end]
+
+    # def replace_text_at_position(self, text:str, replacement:str, start_pos:int, end_pos:int)->str:
+    #     """
+    #     Replance text using text position
         
-        """
-        return text[:start_pos] + replacement + text[end_pos:]
+    #     """
+    #     return text[:start_pos] + replacement + text[end_pos:]
 
     def converting_condition(self, word:str, final_value:list, c_data:list, index:int)-> [list, int]:
 
 
         """
         Convert word to conditional mapping with digits
         """
@@ -222,28 +222,28 @@
             # generate number clustring
             if hundreds_status:
                 clustring_data, clustring_status = self.clustring_consecutive_hunderd(result_chunk)
             else:
                 clustring_data, clustring_status = [result_chunk], [status]
             for c_data, c_status in zip(clustring_data, clustring_status):
                 replance_text = " ".join(c_data)
-                word_spanning = self.find_word_index(original_text, replance_text)
+                word_spanning = npr.find_word_index(original_text, replance_text)
                 index, final_value = 0, []
                 for c_d in c_data:
                     final_value, index = self.converting_condition(c_d, final_value, c_data, index)
                     index += 1
                 value, status = self.adjust_value_conversion(final_value, sum_status= c_status)
                 if status:
                     numbers = str(sum(int(num) for num in value))
                 elif isinstance(value, str):
                     numbers = value
                 else:
                     numbers = "".join(value)
 
-                original_text = self.replace_text_at_position(original_text, numbers, word_spanning[0], word_spanning[1])
+                original_text = npr.replace_text_at_position(original_text, numbers, word_spanning[0], word_spanning[1])
         return original_text
 
     def replace_word_to_number(self, text:list)-> list:
 
         """
         Word to numerical digit conversation
```

### Comparing `pybangla-0.0.4/pybangla/module/parser.py` & `pybangla-1.0.0/pybangla/module/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 import re
 import datetime
 from .config import Config as cfg
 from num2words import num2words
+from .date_extractor import DateExtractor
+# from .number_parser import Word2NumberMap
+
+
+dt = DateExtractor()
+# nr = Normalizer()
 data = cfg.data
 
 _abbreviations = cfg._abbreviations
 _symbols = cfg._symbols
 _ordinal_re = cfg._ordinal_re
 _whitespace_re = cfg._whitespace_re
 _currency = cfg._currency
@@ -138,14 +144,17 @@
         """
         Get weekday name Bangla or English
         
         """
 
         # print("++++++++++++++++++++ : ", date_)
 
+
+        # print("date_: ", date_)
+
         d, y = list(re.finditer(self.bn_regex, str(date_[0]), re.UNICODE)), list(re.finditer(self.bn_regex, str(date_[2]), re.UNICODE))
         
         # print("d, y : ", d, y)
         
         if d:
             date_[0] = self._digit_converter(date_[0], language="bn")
         if y:
@@ -177,14 +186,30 @@
         search_key = int(self._replace_starting_zero(search_key))-1
         month = data[language]["months"][search_key]
         seasons = data[language]["seasons"][search_key//2]
         option_name = data[language]["option_name"][search_key]
 
         return [month, option_name, seasons]
     
+    
+    def find_word_index(self, text:str, word:str)->list:
+        """
+        Word spanning position
+        """
+        start  = text.find(word)
+        end = start+len(word)
+        return [start, end]
+
+    def replace_text_at_position(self, text:str, replacement:str, start_pos:int, end_pos:int)->str:
+        """
+        Replance text using text position
+        
+        """
+        return text[:start_pos] + replacement + text[end_pos:]
+    
     def number_processing(self, text):
 
         # bn_regex, en_regex = r'[০-৯]+', r'[0-9]+'
         bn_matches, en_matches = list(re.finditer(self.bn_regex, text, re.UNICODE)), \
             list(re.finditer(self.en_regex, text, re.UNICODE))
         if en_matches:
             for m in en_matches:
@@ -198,14 +223,16 @@
                     text = text.replace(m[0], bn_m)
         return text
 
 class DateParser:
     def __init__(self):
         self.samples = cfg.samples
 
+        self.npr = NumberParser()
+
     def data_splitter(self, date_string):
         """
         
         """
         separator_pattern = '|'.join(map(re.escape, self.samples))
         return re.split(separator_pattern, date_string)
 
@@ -285,22 +312,60 @@
         for idx, elem in enumerate(date_list):
             if elem.isdigit() and len(elem) == 4:
                 year_idx = idx
                 year = date_list[idx]
                 # print(date_list)
                 day, month = self.get_day_and_month(year_idx, idx, date_list)
         return [day, month, year]
+    
+    def date_processing(self, date_, language="bn"):
+
+        if isinstance(date_, list):
+            if len(date_):
+                formatted_date = date_
+        else:
+            split_date = self.data_splitter(date_)
+            split_date = [i for i in split_date if i]
+
+            if len(split_date)==2:
+                adding_date = ["1"] if language=="en" else ["১"]
+                split_date = adding_date +split_date
+
+            # print("split_date : ", split_date)
+
+            if len(split_date) == 1:
+                formatted_date = self.format_non_punctuation(split_date)
+            else:
+                formatted_date = self.get_date_indexes(split_date)
+
+        if formatted_date[0] == None and formatted_date[1] == None and formatted_date[2] == None:
+            current_date_object = datetime.date.today()
+            formatted_date = [current_date_object.day, current_date_object.month, current_date_object.year]
+
+        weekday = self.npr.get_weekday(formatted_date, language)
+        day   = self.npr._digit_converter(str(formatted_date[0]), language)
+        month = self.npr.search_month(str(formatted_date[1]), language)
+        year  =  self.npr._digit_converter(str(formatted_date[2]), language)
+
+        txt_date = self.npr.number_to_words(day)
+        txt_year = self.npr.year_in_number(year, language=language)
+
+
+        return {"date":day, "month": month[0], "year": year, "txt_date":txt_date, "txt_year": txt_year, "weekday" : weekday, "ls_month": month[1], "seasons" : month[2]}
+
+
 
 class TextParser:
 
     def __init__(self):
         self.year_patterns  =["সালের","সালে", "শতাব্দী", "শতাব্দীর", "শতাব্দীতে"]
         self.year_pattern = r'(?:\b|^\d+)(\d{4})\s*(?:সালে?র?|শতাব্দী(?:র)?|শতাব্দীতে)+'
         self.currency_pattern = r'(?:\$|£|৳|€|¥|₹|₽|₺)?(?:\d+(?:,\d{3})*(?:\.\d+)?|\d+(?:\.\d+)?)'
         self.npr = NumberParser()
+        self.dp = DateParser() 
 
     def collapse_whitespace(self, text):
         return re.sub(_whitespace_re, " ", text)
     
     def expand_symbols(self, text, lang="bn"):
         for regex, replacement in _symbols[lang]:
             # print("regex : ", regex)
@@ -365,34 +430,43 @@
             # print(currency)
             if currency:
                 # print("m : ", m)
                 n_m = m.replace(currency[0], "")
                 if "." in n_m:
                     s_m = n_m.split(".")
                     before_dot_word, after_dot_word = self.npr.number_to_words(s_m[0]), self.npr.digit_number_to_digit_word(s_m[1])
-
                     word =  before_dot_word+" দশমি "+after_dot_word+ " "+_currency[currency[0]]
                     text = text.replace(m, word)
                     # print(s_m, before_dot_word, after_dot_word)
                 else:
                     word = self.npr.number_to_words(n_m)
                     n_word = word + " "+_currency[currency[0]]
-
-
                     text = text.replace(m, n_word)
         return text
     
+    def replance_date_processing(self, text):
+        dates = dt.get_dates(text)
+        for date in dates:
+            position = self.npr.find_word_index(text, date)
+            formated_date = self.dp.date_processing(date)
+            # print(formated_date)
+            f_d_string = formated_date["txt_date"]+" "+formated_date["month"]+" "+formated_date["txt_year"]
+            # print(f_d_string)
+            text = self.npr.replace_text_at_position(text, f_d_string, position[0], position[1])
+        return text
+
+    
 
     def processing(self, text):
         text = self.collapse_whitespace(text)
         text = self.expand_symbols(text)
         text = self.expand_abbreviations(text)
         text = self.expand_position(text)
         text = self.extract_currency_amounts(text)
-        text = self.year_formation(text)
+        text = self.replance_date_processing(text)
         text = self.npr.number_processing(text)
         return text
     
 if __name__ =="__main__":
 
     text = "রাহিম ক্লাস ওয়ান এ ১ম, ১১তম ২২ তম ৩৩ তম, ১২৩৪ শতাব্দীতে ¥২০৩০.১২৩৪ বিবিধ  বাকেরগঞ্জ উপজেলার প্রায় 40 ভাগের পেশাই চাষাবাদ 80 and 40 ২২"
     tp = TextParser()
```

### Comparing `pybangla-0.0.4/pybangla/module/word_to_number.py` & `pybangla-1.0.0/pybangla/module/word_to_number.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.4/pybangla.egg-info/PKG-INFO` & `pybangla-1.0.0/pybangla.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 0.0.4
+Version: 1.0.0
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: DateTime
 Requires-Dist: num2words
 
 
-PYBANGLA is a python3 package for Bengala Number, DateTime and Text Normalizer. This package can be used Normalize the text number and date (ex: number to text vice versa). This framework  also can be used Django, Flask, FastAPI, and others. PYBANGLA module supported operating system Linux/Unix, Mac OS and Windows.
+PYBANGLA is a python3 package for Bangla Number, DateTime and Text Normalizer and Date Extraction. This package can be used Normalize the text number and date (ex: number to text vice versa). This framework  also can be used Django, Flask, FastAPI, and others. PYBANGLA module supported operating system Linux/Unix, Mac OS and Windows.
 Available Features
 
 Features available in PYBANGLA:
 
 1. Text Normalization
 2. Number Conversion
 3. Date Format
@@ -31,16 +31,14 @@
 The easiest way to install pybangla is to use pip:
 
 ```
 pip install pybangla
 ```
 
 
-
-
 # Usage
 
 ## 1. Text Normalization
 ### It supports converting Bangla abbreviations, symbols, and currencies to Bangla textual format.
 
 ```py
 import pybangla
@@ -70,14 +68,24 @@
 text = "আজকের তাপমাত্রা ৪৪°"
 
 #output:
 'আজকের তাপমাত্রা চুয়াল্লিশ ডিগ্রী'
 
 ```
 
+```py
+
+text = "সম্মেলনটি সেপ্টেম্বর ০৫ ২০২৩ তারিখে নির্ধারিত করা হয়েছে. এপ্রিল ২০২৩"
+text = nrml.text_normalizer(text)
+#output:
+
+সম্মেলনটি পাঁচ সেপ্টেম্বর দুই হাজার তেইশ তারিখে নির্ধারিত করা হয়েছে. এক এপ্রিল দুই হাজার তেইশ
+
+```
+
 Supported
 
 ```
 #abbreviations:
 ("সাঃ", "সাল্লাল্লাহু আলাইহি ওয়া সাল্লাম"),                  
 ("আঃ", "আলাইহিস সালাম"),
 ("রাঃ", "রাদিআল্লাহু আনহু"),
@@ -284,34 +292,54 @@
 {'date': '০৪', 'month': 'জানুয়ারি', 'year': '২০২৩', 'weekday': 'বুধবার', 'ls_month': 'বৈশাখ', 'seasons': 'গ্রীষ্ম'}
 
 or
 English:
 
 {'date': '04', 'month': 'January', 'year': '2023', 'weekday': 'Wednesday', 'ls_month': 'Jan', 'seasons': 'Summer'}
 ```
-```
+```py
 import pybangla
 nrml = pybangla.Normalizer()
 
 date = dt.date_format("01-Apr/2023", language="bn")
 print(f"{date}")
 # Output: 
 {'date': '০১', 'month': 'এপ্রিল', 'year': '২০২৩', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
 ```
 
-```
+```py
 import pybangla
 nrml = pybangla.Normalizer()
 en_date = dt.date_format("01-Apr/2023", language="en")
 print(f"{en_date}")
 
 # Output :
 {'date': '01', 'month': 'April', 'year': '2023', 'weekday': 'Saturday', 'ls_month': 'Apr', 'seasons': 'Wet season'}
 ```
 
+## Date extraction
+
+```py
+Rule based Date Extraction
+import pybangla
+nrml = pybangla.Normalizer()
+
+text = "সম্মেলনটি সেপ্টেম্বর ০৫ ২০২৩ তারিখে নির্ধারিত করা হয়েছে. এপ্রিল ২০২৩"
+dates = nrml.date_extraction(text)
+
+#output:
+
+[
+{'date': '০৫', 'month': 'সেপ্টেম্বর', 'year': '২০২৩', 'txt_date': 'পাঁচ', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'মঙ্গলবার', 'ls_month': 'পৌষ', 'seasons': 'শীত'}, 
+
+{'date': '১', 'month': 'এপ্রিল', 'year': '২০২৩', 'txt_date': 'এক', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
+]
+
+```
+
 ## 4. Today, Months, Weekdays, Seasons
 ### It converts Bangla (today, months, weekdays, and seasons) to English and English to Bangla, and vice versa, in a pair format.
 
 ## 1. Today:
 
 ```py
 import pybangla
@@ -469,15 +497,23 @@
 ```
 # Next Upcomming Features
 
 1. Date extraction from normal text sentence and convert it numerical to word(vice versa)
 2. Bangla lemmatization and stemming algorithm
 3. Bangla Tokenizer
 
-# Contribute
-
-If you face any problem feel free to open issue.
 
 # Contact
 If you have any suggestion: Email: saifulbrur79@gmail.com
 
+# Contributor
+
+```
+@misc{BanglaASR ,
+  title={PYBANGLA module use for normalize textual format like text to number and number to text},
+  author={Md Saiful Islam, Hassan Ali Emon,  HM-badhon, Sagor Sarker},
+  howpublished={},
+  year={2024}
+}
+```
+If you face any problem feel free to open issue.
```

### Comparing `pybangla-0.0.4/setup.py` & `pybangla-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import codecs
 from setuptools import setup, find_packages
 
 setup(
     name='pybangla',
-    version='0.0.4',
+    version='1.0.0',
     packages=find_packages(),
     # entry_points={
     #     'console_scripts': [
     #         'pybangla = pybangla.main:Normalizer'
     #     ]
     # },
     author='saiful',
```

### Comparing `pybangla-0.0.4/tests/test.py` & `pybangla-1.0.0/tests/test.py`

 * *Files identical despite different names*

