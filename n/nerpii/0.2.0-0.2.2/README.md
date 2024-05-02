# Comparing `tmp/nerpii-0.2.0.tar.gz` & `tmp/nerpii-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerpii-0.2.0.tar", max compression
+gzip compressed data, was "nerpii-0.2.2.tar", max compression
```

## Comparing `nerpii-0.2.0.tar` & `nerpii-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3106 2024-01-29 16:29:35.274909 nerpii-0.2.0/README.md
--rw-r--r--   0        0        0      209 2024-01-29 16:29:35.274909 nerpii-0.2.0/nerpii/__init__.py
--rw-r--r--   0        0        0    22243 2024-01-29 16:29:35.274909 nerpii-0.2.0/nerpii/faker_generator.py
--rw-r--r--   0        0        0    18421 2024-01-29 16:29:35.274909 nerpii-0.2.0/nerpii/named_entity_recognizer.py
--rw-r--r--   0        0        0      840 2024-01-29 16:29:35.278909 nerpii-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4078 1970-01-01 00:00:00.000000 nerpii-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3106 2024-05-02 08:19:42.839183 nerpii-0.2.2/README.md
+-rw-r--r--   0        0        0      209 2024-05-02 08:19:42.839183 nerpii-0.2.2/nerpii/__init__.py
+-rw-r--r--   0        0        0    22243 2024-05-02 08:19:42.839183 nerpii-0.2.2/nerpii/faker_generator.py
+-rw-r--r--   0        0        0    18421 2024-05-02 08:19:42.839183 nerpii-0.2.2/nerpii/named_entity_recognizer.py
+-rw-r--r--   0        0        0      841 2024-05-02 08:19:42.843183 nerpii-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4071 1970-01-01 00:00:00.000000 nerpii-0.2.2/PKG-INFO
```

### Comparing `nerpii-0.2.0/README.md` & `nerpii-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nerpii-0.2.0/nerpii/faker_generator.py` & `nerpii-0.2.2/nerpii/faker_generator.py`

 * *Files identical despite different names*

### Comparing `nerpii-0.2.0/nerpii/named_entity_recognizer.py` & `nerpii-0.2.2/nerpii/named_entity_recognizer.py`

 * *Files identical despite different names*

### Comparing `nerpii-0.2.0/pyproject.toml` & `nerpii-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nerpii"
-version = "0.2.0"
+version = "0.2.2"
 description = "A python library to perform NER on structured data and generate PII with Faker"
 authors = ["Clearbox AI <info@clearbox.ai>"]
 license = "GPL"
 readme = "README.md"
 homepage = "https://github.com/Clearbox-AI/nerpii"
 repository = "https://github.com/Clearbox-AI/nerpii"
 packages = [{include = "nerpii"}]
@@ -14,15 +14,15 @@
 pandas = "^1.5.3"
 presidio-analyzer = "^2.2.32"
 transformers = "^4.26.1"
 faker = "^17.3.0"
 gender-guesser = "^0.4.0"
 simple-colors = "^0.1.5"
 spacy = "3.5.0"
-torch = "^1.13.1"
+torch = ">=1.13.1"
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.21.1"
 pytest = "^7.2.1"
 flake8 = "^6.0.0"
 flake8-import-order = "^0.18.2"
```

### Comparing `nerpii-0.2.0/PKG-INFO` & `nerpii-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerpii
-Version: 0.2.0
+Version: 0.2.2
 Summary: A python library to perform NER on structured data and generate PII with Faker
 Home-page: https://github.com/Clearbox-AI/nerpii
 License: GPL
 Author: Clearbox AI
 Author-email: info@clearbox.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faker (>=17.3.0,<18.0.0)
 Requires-Dist: gender-guesser (>=0.4.0,<0.5.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: presidio-analyzer (>=2.2.32,<3.0.0)
 Requires-Dist: simple-colors (>=0.1.5,<0.2.0)
 Requires-Dist: spacy (==3.5.0)
-Requires-Dist: torch (>=1.13.1,<2.0.0)
+Requires-Dist: torch (>=1.13.1)
 Requires-Dist: transformers (>=4.26.1,<5.0.0)
 Project-URL: Repository, https://github.com/Clearbox-AI/nerpii
 Description-Content-Type: text/markdown
 
 # Nerpii 
 Nerpii is a Python library developed to perform Named Entity Recognition (NER) on structured datasets and synthesize Personal Identifiable Information (PII).
```

