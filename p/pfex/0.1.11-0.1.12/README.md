# Comparing `tmp/pfex-0.1.11.tar.gz` & `tmp/pfex-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfex-0.1.11.tar", last modified: Thu May  2 20:51:37 2024, max compression
+gzip compressed data, was "pfex-0.1.12.tar", last modified: Thu May  2 20:54:41 2024, max compression
```

## Comparing `pfex-0.1.11.tar` & `pfex-0.1.12.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2024-05-02 20:51:37.453943 pfex-0.1.11/
--rw-r--r--   0 maayanlab   (501) staff       (20)    14637 2024-05-02 20:50:29.000000 pfex-0.1.11/LICENSE
--rw-r--r--   0 maayanlab   (501) staff       (20)     6432 2024-05-02 20:51:37.453812 pfex-0.1.11/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)     5924 2024-05-02 20:50:29.000000 pfex-0.1.11/README.md
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2024-05-02 20:51:37.451938 pfex-0.1.11/pfex/
--rw-r--r--   0 maayanlab   (501) staff       (20)      162 2024-05-02 20:50:29.000000 pfex-0.1.11/pfex/__init__.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2024-05-02 20:51:37.453622 pfex-0.1.11/pfex/data/
--rw-r--r--   0 maayanlab   (501) staff       (20)  1380288 2024-05-02 20:50:29.000000 pfex-0.1.11/pfex/data/GO_Biological_Process_2023
--rw-r--r--   0 maayanlab   (501) staff       (20)      178 2024-05-02 20:50:29.000000 pfex-0.1.11/pfex/data/config.json
--rw-r--r--   0 maayanlab   (501) staff       (20)     1205 2024-05-02 20:50:29.000000 pfex-0.1.11/pfex/data/example_gene_set.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)     6876 2024-05-02 20:50:29.000000 pfex-0.1.11/pfex/enrichment.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     4724 2024-05-02 20:50:29.000000 pfex-0.1.11/pfex/libraries.py
--rw-r--r--   0 maayanlab   (501) staff       (20)      958 2024-05-02 20:50:29.000000 pfex-0.1.11/pfex/modules.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2024-05-02 20:51:37.452556 pfex-0.1.11/pfex.egg-info/
--rw-r--r--   0 maayanlab   (501) staff       (20)     6432 2024-05-02 20:51:37.000000 pfex-0.1.11/pfex.egg-info/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)      325 2024-05-02 20:51:37.000000 pfex-0.1.11/pfex.egg-info/SOURCES.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        1 2024-05-02 20:51:37.000000 pfex-0.1.11/pfex.egg-info/dependency_links.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)       62 2024-05-02 20:51:37.000000 pfex-0.1.11/pfex.egg-info/requires.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        5 2024-05-02 20:51:37.000000 pfex-0.1.11/pfex.egg-info/top_level.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)       38 2024-05-02 20:51:37.454004 pfex-0.1.11/setup.cfg
--rw-r--r--   0 maayanlab   (501) staff       (20)      965 2024-05-02 20:50:29.000000 pfex-0.1.11/setup.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2024-05-02 20:54:41.853184 pfex-0.1.12/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    14637 2024-05-02 20:50:29.000000 pfex-0.1.12/LICENSE
+-rw-r--r--   0 maayanlab   (501) staff       (20)     6375 2024-05-02 20:54:41.853058 pfex-0.1.12/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)     5866 2024-05-02 20:54:29.000000 pfex-0.1.12/README.md
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2024-05-02 20:54:41.851100 pfex-0.1.12/pfex/
+-rw-r--r--   0 maayanlab   (501) staff       (20)      162 2024-05-02 20:50:29.000000 pfex-0.1.12/pfex/__init__.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2024-05-02 20:54:41.852883 pfex-0.1.12/pfex/data/
+-rw-r--r--   0 maayanlab   (501) staff       (20)  1380288 2024-05-02 20:50:29.000000 pfex-0.1.12/pfex/data/GO_Biological_Process_2023
+-rw-r--r--   0 maayanlab   (501) staff       (20)      178 2024-05-02 20:50:29.000000 pfex-0.1.12/pfex/data/config.json
+-rw-r--r--   0 maayanlab   (501) staff       (20)     1205 2024-05-02 20:50:29.000000 pfex-0.1.12/pfex/data/example_gene_set.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)     6876 2024-05-02 20:50:29.000000 pfex-0.1.12/pfex/enrichment.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     4724 2024-05-02 20:50:29.000000 pfex-0.1.12/pfex/libraries.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)      958 2024-05-02 20:50:29.000000 pfex-0.1.12/pfex/modules.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2024-05-02 20:54:41.851753 pfex-0.1.12/pfex.egg-info/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     6375 2024-05-02 20:54:41.000000 pfex-0.1.12/pfex.egg-info/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)      325 2024-05-02 20:54:41.000000 pfex-0.1.12/pfex.egg-info/SOURCES.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        1 2024-05-02 20:54:41.000000 pfex-0.1.12/pfex.egg-info/dependency_links.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)       67 2024-05-02 20:54:41.000000 pfex-0.1.12/pfex.egg-info/requires.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        5 2024-05-02 20:54:41.000000 pfex-0.1.12/pfex.egg-info/top_level.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)       38 2024-05-02 20:54:41.853236 pfex-0.1.12/setup.cfg
+-rw-r--r--   0 maayanlab   (501) staff       (20)      982 2024-05-02 20:54:11.000000 pfex-0.1.12/setup.py
```

### Comparing `pfex-0.1.11/LICENSE` & `pfex-0.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `pfex-0.1.11/PKG-INFO` & `pfex-0.1.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pfex
-Version: 0.1.11
+Version: 0.1.12
 Summary: Package for fast and accurate calculation of Fisher Exact Test with Enrichr library support.
-Home-page: https://github.com/maayanlab/pfx
+Home-page: https://github.com/maayanlab/pfex
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -17,15 +17,15 @@
 The Python Fisher Exact test package supports EnrichR libraries and mimics the EnrichR backend. It has high performance for large gene set libraries. Instant enrichment results for a pure Python implementation of the Fisher Exact Test. This implementation allows the calculation of the same p-values as the Enrichr API, but runs locally and results in faster p-value computation.
 
 ### Installation
 
 Install Python library using pip directly from Github. The repository is currently private.
 
 ```
-pip3 install git+https://<token>:x-oauth-basic@github.com/maayanlab/pfx.git
+pip3 install pfex
 ```
 
 Replace <token> with the Github token allowing access. You can generate an access token in Github by selecting Profile (top right -> Settings -> Developer Settings -> Personal Access Tokens)
 
 
 ### Enrichment Analysis
```

### Comparing `pfex-0.1.11/README.md` & `pfex-0.1.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 The Python Fisher Exact test package supports EnrichR libraries and mimics the EnrichR backend. It has high performance for large gene set libraries. Instant enrichment results for a pure Python implementation of the Fisher Exact Test. This implementation allows the calculation of the same p-values as the Enrichr API, but runs locally and results in faster p-value computation.
 
 ### Installation
 
 Install Python library using pip directly from Github. The repository is currently private.
 
 ```
-pip3 install git+https://<token>:x-oauth-basic@github.com/maayanlab/pfx.git
+pip3 install pfex
 ```
 
 Replace <token> with the Github token allowing access. You can generate an access token in Github by selecting Profile (top right -> Settings -> Developer Settings -> Personal Access Tokens)
 
 
 ### Enrichment Analysis
```

### Comparing `pfex-0.1.11/pfex/data/GO_Biological_Process_2023` & `pfex-0.1.12/pfex/data/GO_Biological_Process_2023`

 * *Files identical despite different names*

### Comparing `pfex-0.1.11/pfex/data/example_gene_set.txt` & `pfex-0.1.12/pfex/data/example_gene_set.txt`

 * *Files identical despite different names*

### Comparing `pfex-0.1.11/pfex/enrichment.py` & `pfex-0.1.12/pfex/enrichment.py`

 * *Files identical despite different names*

### Comparing `pfex-0.1.11/pfex/libraries.py` & `pfex-0.1.12/pfex/libraries.py`

 * *Files identical despite different names*

### Comparing `pfex-0.1.11/pfex/modules.py` & `pfex-0.1.12/pfex/modules.py`

 * *Files identical despite different names*

### Comparing `pfex-0.1.11/pfex.egg-info/PKG-INFO` & `pfex-0.1.12/pfex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pfex
-Version: 0.1.11
+Version: 0.1.12
 Summary: Package for fast and accurate calculation of Fisher Exact Test with Enrichr library support.
-Home-page: https://github.com/maayanlab/pfx
+Home-page: https://github.com/maayanlab/pfex
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -17,15 +17,15 @@
 The Python Fisher Exact test package supports EnrichR libraries and mimics the EnrichR backend. It has high performance for large gene set libraries. Instant enrichment results for a pure Python implementation of the Fisher Exact Test. This implementation allows the calculation of the same p-values as the Enrichr API, but runs locally and results in faster p-value computation.
 
 ### Installation
 
 Install Python library using pip directly from Github. The repository is currently private.
 
 ```
-pip3 install git+https://<token>:x-oauth-basic@github.com/maayanlab/pfx.git
+pip3 install pfex
 ```
 
 Replace <token> with the Github token allowing access. You can generate an access token in Github by selecting Profile (top right -> Settings -> Developer Settings -> Personal Access Tokens)
 
 
 ### Enrichment Analysis
```

### Comparing `pfex-0.1.11/setup.py` & `pfex-0.1.12/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pfex",
-    version="0.1.11",
+    version="0.1.12",
     author="Alexander Lachmann",
     author_email="alexander.lachmann@mssm.edu",
     description="Package for fast and accurate calculation of Fisher Exact Test with Enrichr library support.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/maayanlab/pfx",
+    url="https://github.com/maayanlab/pfex",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     package_data={
@@ -24,11 +24,12 @@
     include_package_data=True,
     install_requires=[
         'pandas>=1.1.5',
         'numpy',
         'statsmodels',
         'numba',
         'python-louvain',
-        'networkx'
+        'networkx',
+        'tqdm'
     ],
     python_requires='>=3.6',
 )
```

