# Comparing `tmp/broad_babel-0.1.8.tar.gz` & `tmp/broad_babel-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "broad_babel-0.1.8.tar", max compression
+gzip compressed data, was "broad_babel-0.1.9.tar", max compression
```

## Comparing `broad_babel-0.1.8.tar` & `broad_babel-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     2490 2023-12-16 04:47:11.069602 broad_babel-0.1.8/README.md
--rw-r--r--   0        0        0      698 2023-12-16 23:53:57.252464 broad_babel-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       23 2023-12-07 18:31:33.798266 broad_babel-0.1.8/src/broad_babel/__init__.py
--rw-r--r--   0        0        0     3676 2023-12-16 04:47:11.070863 broad_babel-0.1.8/src/broad_babel/query.py
--rw-r--r--   0        0        0      312 2023-12-16 04:42:21.288356 broad_babel-0.1.8/src/broad_babel/test.py
--rw-r--r--   0        0        0     3079 1970-01-01 00:00:00.000000 broad_babel-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2556 2024-01-03 22:31:44.000000 broad_babel-0.1.9/README.md
+-rw-r--r--   0        0        0      698 2024-01-03 22:38:49.000000 broad_babel-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-12-20 04:47:29.000000 broad_babel-0.1.9/src/broad_babel/__init__.py
+-rw-r--r--   0        0        0     3676 2024-01-03 22:30:45.000000 broad_babel-0.1.9/src/broad_babel/query.py
+-rw-r--r--   0        0        0     3145 1970-01-01 00:00:00.000000 broad_babel-0.1.9/PKG-INFO
```

### Comparing `broad_babel-0.1.8/README.md` & `broad_babel-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ## Custom querying
 The available fields are:
 - perturbation: Dataset of origin for a given entry
 - JCP2022: Identifier from the JUMP dataset
 - standard_key: Gene Entrez id for gene-related perturbations, and InChIKey for compound perturbations
 - broad_sample: Internal Broad ID
 - pert_type: Type of perturbation, options are trt (treatment), control, negcon (Negative Control), poscon_cp (Positive Control, Compound Probe), poscon_diverse, poscon_orf, and poscon (Positive Control).
-
+- NCBI_Gene_ID: NCBI identifier, only applicable to ORF and CRISPR
 
 You can fetch any field using another (note that the output is a list of tuples)
 
 ```python
 run_query(query="JCP2022_915119", input_column="JCP2022", output_column="broad_sample")
 # [('ccsbBroad304_16164',)]
 ```
```

### Comparing `broad_babel-0.1.8/pyproject.toml` & `broad_babel-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "broad-babel"
-version = "0.1.8"
+version = "0.1.9"
 description = "A translator of Broad and JUMP ids to more conventional names."
 authors = ["Alan Munoz"]
 readme = "README.md"
 packages = [{include = "broad_babel", from= "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `broad_babel-0.1.8/src/broad_babel/query.py` & `broad_babel-0.1.9/src/broad_babel/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import pooch
 
 DB_FILE = pooch.retrieve(
     # Temporarily commented out due to Zenodo API change
     # url="doi:10.5281/zenodo.8350361/names.db",
     # url=("https://zenodo.org/records/8350361/files/" "names.db"),
     # known_hash="md5:80f0f5b8ea8c01a911c1a9196dcbd2fd",
-    url=("https://zenodo.org/records/10393656/files/" "babel.db"),
-    known_hash="md5:df52c4843ef9cf914db55b9d85f304d4",
+    url=("https://zenodo.org/records/10456863/files/" "babel.db"),
+    known_hash="md5:2eee333428a78b034b384e04352f72da",
 )
 TABLE = "babel"
 
 
 @cache
 def run_query(
     query: str or tuple[str],
```

### Comparing `broad_babel-0.1.8/PKG-INFO` & `broad_babel-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: broad-babel
-Version: 0.1.8
+Version: 0.1.9
 Summary: A translator of Broad and JUMP ids to more conventional names.
 Author: Alan Munoz
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -49,15 +49,15 @@
 ## Custom querying
 The available fields are:
 - perturbation: Dataset of origin for a given entry
 - JCP2022: Identifier from the JUMP dataset
 - standard_key: Gene Entrez id for gene-related perturbations, and InChIKey for compound perturbations
 - broad_sample: Internal Broad ID
 - pert_type: Type of perturbation, options are trt (treatment), control, negcon (Negative Control), poscon_cp (Positive Control, Compound Probe), poscon_diverse, poscon_orf, and poscon (Positive Control).
-
+- NCBI_Gene_ID: NCBI identifier, only applicable to ORF and CRISPR
 
 You can fetch any field using another (note that the output is a list of tuples)
 
 ```python
 run_query(query="JCP2022_915119", input_column="JCP2022", output_column="broad_sample")
 # [('ccsbBroad304_16164',)]
 ```
```

