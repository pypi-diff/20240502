# Comparing `tmp/laser_encoders-0.0.1.tar.gz` & `tmp/laser_encoders-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laser_encoders-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "laser_encoders-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `laser_encoders-0.0.1.tar` & `laser_encoders-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     6126 2023-11-21 15:56:22.702684 laser_encoders-0.0.1/laser_encoders/README.md
--rw-r--r--   0        0        0      610 2023-11-21 15:56:22.705504 laser_encoders-0.0.1/laser_encoders/__init__.py
--rw-r--r--   0        0        0     5134 2023-11-21 15:56:22.708451 laser_encoders-0.0.1/laser_encoders/download_models.py
--rw-r--r--   0        0        0    16981 2023-11-21 15:56:22.712197 laser_encoders-0.0.1/laser_encoders/language_list.py
--rw-r--r--   0        0        0     6400 2023-11-21 15:56:22.716858 laser_encoders-0.0.1/laser_encoders/laser_tokenizer.py
--rw-r--r--   0        0        0    15125 2023-11-21 15:56:22.720561 laser_encoders-0.0.1/laser_encoders/models.py
--rw-r--r--   0        0        0    10023 2023-11-21 15:56:22.724233 laser_encoders-0.0.1/laser_encoders/test_laser_tokenizer.py
--rw-r--r--   0        0        0     2129 2023-11-21 15:56:22.727302 laser_encoders-0.0.1/laser_encoders/test_models_initialization.py
--rw-r--r--   0        0        0     3915 2023-11-21 15:56:22.730258 laser_encoders-0.0.1/laser_encoders/validate_models.py
--rw-r--r--   0        0        0     1517 2023-11-21 15:56:22.734852 laser_encoders-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7234 1970-01-01 00:00:00.000000 laser_encoders-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6126 2023-11-21 15:56:22.702684 laser_encoders-0.0.2/laser_encoders/README.md
+-rw-r--r--   0        0        0      610 2023-11-21 15:56:22.705504 laser_encoders-0.0.2/laser_encoders/__init__.py
+-rw-r--r--   0        0        0     5385 2024-05-02 20:21:55.142578 laser_encoders-0.0.2/laser_encoders/download_models.py
+-rw-r--r--   0        0        0    16981 2023-11-21 16:22:09.925810 laser_encoders-0.0.2/laser_encoders/language_list.py
+-rw-r--r--   0        0        0     6400 2023-11-21 16:22:09.929454 laser_encoders-0.0.2/laser_encoders/laser_tokenizer.py
+-rw-r--r--   0        0        0    15125 2023-11-21 16:22:09.933968 laser_encoders-0.0.2/laser_encoders/models.py
+-rw-r--r--   0        0        0    10023 2023-11-21 16:22:09.938166 laser_encoders-0.0.2/laser_encoders/test_laser_tokenizer.py
+-rw-r--r--   0        0        0     2129 2023-11-21 15:56:22.727302 laser_encoders-0.0.2/laser_encoders/test_models_initialization.py
+-rw-r--r--   0        0        0     3915 2023-11-21 15:56:22.730258 laser_encoders-0.0.2/laser_encoders/validate_models.py
+-rw-r--r--   0        0        0     1517 2024-05-02 20:23:02.075778 laser_encoders-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7234 1970-01-01 00:00:00.000000 laser_encoders-0.0.2/PKG-INFO
```

### Comparing `laser_encoders-0.0.1/laser_encoders/README.md` & `laser_encoders-0.0.2/laser_encoders/README.md`

 * *Files identical despite different names*

### Comparing `laser_encoders-0.0.1/laser_encoders/__init__.py` & `laser_encoders-0.0.2/laser_encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `laser_encoders-0.0.1/laser_encoders/download_models.py` & `laser_encoders-0.0.2/laser_encoders/download_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,18 @@
             model_dir = os.path.expanduser("~/.cache/laser_encoders")
             os.makedirs(model_dir, exist_ok=True)
 
         self.model_dir = Path(model_dir)
         self.base_url = "https://dl.fbaipublicfiles.com/nllb/laser"
 
     def download(self, filename: str):
-        url = os.path.join(self.base_url, filename)
+        # Because on windows os.path.join will use "\" insted of "/", so link would be:
+        # https://dl.fbaipublicfiles.com/nllb/laser\laser2.pt instead of https://dl.fbaipublicfiles.com/nllb/laser/laser2.pt
+        # which results in a failed download.
+        url = f"{self.base_url}/{filename}"
         local_file_path = os.path.join(self.model_dir, filename)
 
         if os.path.exists(local_file_path):
             logger.info(f" - {filename} already downloaded")
         else:
             logger.info(f" - Downloading {filename}")
```

### Comparing `laser_encoders-0.0.1/laser_encoders/language_list.py` & `laser_encoders-0.0.2/laser_encoders/language_list.py`

 * *Files identical despite different names*

### Comparing `laser_encoders-0.0.1/laser_encoders/laser_tokenizer.py` & `laser_encoders-0.0.2/laser_encoders/laser_tokenizer.py`

 * *Files identical despite different names*

### Comparing `laser_encoders-0.0.1/laser_encoders/models.py` & `laser_encoders-0.0.2/laser_encoders/models.py`

 * *Files identical despite different names*

### Comparing `laser_encoders-0.0.1/laser_encoders/test_laser_tokenizer.py` & `laser_encoders-0.0.2/laser_encoders/test_laser_tokenizer.py`

 * *Files identical despite different names*

### Comparing `laser_encoders-0.0.1/laser_encoders/test_models_initialization.py` & `laser_encoders-0.0.2/laser_encoders/test_models_initialization.py`

 * *Files identical despite different names*

### Comparing `laser_encoders-0.0.1/laser_encoders/validate_models.py` & `laser_encoders-0.0.2/laser_encoders/validate_models.py`

 * *Files identical despite different names*

### Comparing `laser_encoders-0.0.1/pyproject.toml` & `laser_encoders-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4", "setuptools"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "laser_encoders"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{name = "Facebook AI Research"}]
 description = "LASER  Language-Agnostic SEntence Representations is a toolkit to calculate multilingual sentence embeddings and to use them for document classification, bitext filtering and mining"
 readme = "laser_encoders/README.md"
 requires-python = ">=3.8"
 
 dependencies = [
     'sacremoses==0.1.0',
```

### Comparing `laser_encoders-0.0.1/PKG-INFO` & `laser_encoders-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laser_encoders
-Version: 0.0.1
+Version: 0.0.2
 Summary: LASER  Language-Agnostic SEntence Representations is a toolkit to calculate multilingual sentence embeddings and to use them for document classification, bitext filtering and mining
 Author: Facebook AI Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Development Status :: 4 - Beta
```

