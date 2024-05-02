# Comparing `tmp/aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714554917.tar.gz` & `tmp/aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714641537.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714554917.tar", max compression
+gzip compressed data, was "aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714641537.tar", max compression
```

## Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714554917.tar` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714641537.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     9580 2024-05-01 09:14:38.832671 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714554917/LICENSE
--rw-r--r--   0        0        0        0 2024-05-01 08:12:08.757010 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714554917/README.md
--rw-r--r--   0        0        0      791 2024-05-01 09:15:18.103627 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714554917/pyproject.toml
--rw-r--r--   0        0        0     8837 2024-05-01 08:12:08.758010 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714554917/src/model_training_api_sagemaker/model_training_api_sagemaker.py
--rw-r--r--   0        0        0      632 1970-01-01 00:00:00.000000 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714554917/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-02 09:18:17.244006 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714641537/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-02 08:12:10.074802 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714641537/README.md
+-rw-r--r--   0        0        0      791 2024-05-02 09:18:57.538950 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714641537/pyproject.toml
+-rw-r--r--   0        0        0     8837 2024-05-02 08:12:10.074802 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714641537/src/model_training_api_sagemaker/model_training_api_sagemaker.py
+-rw-r--r--   0        0        0      632 1970-01-01 00:00:00.000000 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714641537/PKG-INFO
```

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714554917/LICENSE` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714641537/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714554917/pyproject.toml` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714641537/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-extensions-model-training-api-sagemaker"
-version = "1.7.0.dev1714554917"
+version = "1.7.0.dev1714641537"
 description = ""
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "model_training_api_sagemaker", from = "src"},
 ]
```

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714554917/src/model_training_api_sagemaker/model_training_api_sagemaker.py` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714641537/src/model_training_api_sagemaker/model_training_api_sagemaker.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714554917/PKG-INFO` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714641537/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-extensions-model-training-api-sagemaker
-Version: 1.7.0.dev1714554917
+Version: 1.7.0.dev1714641537
 Summary: 
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<3.12
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: fastapi (>=0.95.0)
 Requires-Dist: krausening (>=19)
```

