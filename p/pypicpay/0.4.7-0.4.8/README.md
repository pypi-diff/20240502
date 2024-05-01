# Comparing `tmp/pypicpay-0.4.7.tar.gz` & `tmp/pypicpay-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypicpay-0.4.7.tar", max compression
+gzip compressed data, was "pypicpay-0.4.8.tar", max compression
```

## Comparing `pypicpay-0.4.7.tar` & `pypicpay-0.4.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2024-03-29 20:55:40.702692 pypicpay-0.4.7/LICENSE
--rw-r--r--   0        0        0     7834 2024-03-29 20:55:40.702899 pypicpay-0.4.7/README.md
--rw-r--r--   0        0        0       64 2024-03-30 21:48:16.565482 pypicpay-0.4.7/pypicpay/__init__.py
--rw-r--r--   0        0        0     7026 2024-03-29 20:55:40.704504 pypicpay-0.4.7/pypicpay/picpay.py
--rw-r--r--   0        0        0      790 2024-03-30 21:48:11.530934 pypicpay-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     8650 1970-01-01 00:00:00.000000 pypicpay-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-29 20:55:40.702692 pypicpay-0.4.8/LICENSE
+-rw-r--r--   0        0        0     7834 2024-05-01 23:38:58.061431 pypicpay-0.4.8/README.md
+-rw-r--r--   0        0        0       64 2024-05-01 23:38:56.091383 pypicpay-0.4.8/pypicpay/__init__.py
+-rw-r--r--   0        0        0     7026 2024-03-29 20:55:40.704504 pypicpay-0.4.8/pypicpay/picpay.py
+-rw-r--r--   0        0        0      790 2024-05-01 23:38:55.934437 pypicpay-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     8650 1970-01-01 00:00:00.000000 pypicpay-0.4.8/PKG-INFO
```

### Comparing `pypicpay-0.4.7/LICENSE` & `pypicpay-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypicpay-0.4.7/README.md` & `pypicpay-0.4.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -161,12 +161,12 @@
 
 ```bash
 $ pytest
 ```
 
 # Dependências
 
-- [Python >=3.8](https://www.python.org/downloads/release/python-388/)
+- [Python >=3.7](https://www.python.org/downloads/release/python-370/)
 
 # Licença
 
 [MIT](https://en.wikipedia.org/wiki/MIT_License)
```

### Comparing `pypicpay-0.4.7/pypicpay/picpay.py` & `pypicpay-0.4.8/pypicpay/picpay.py`

 * *Files identical despite different names*

### Comparing `pypicpay-0.4.7/pyproject.toml` & `pypicpay-0.4.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypicpay"
-version = "0.4.7"
+version = "0.4.8"
 description = "Aceite PicPay e faça parte do movimento que está revolucionando a relação com o dinheiro no Brasil."
 authors = ["Hudson Brendon <contato.hudsonbrendon@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/hudsonbrendon/picpay"
 homepage = "https://github.com/hudsonbrendon/picpay#readme"
```

### Comparing `pypicpay-0.4.7/PKG-INFO` & `pypicpay-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypicpay
-Version: 0.4.7
+Version: 0.4.8
 Summary: Aceite PicPay e faça parte do movimento que está revolucionando a relação com o dinheiro no Brasil.
 Home-page: https://github.com/hudsonbrendon/picpay#readme
 License: MIT
 Author: Hudson Brendon
 Author-email: contato.hudsonbrendon@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -181,13 +181,13 @@
 
 ```bash
 $ pytest
 ```
 
 # Dependências
 
-- [Python >=3.8](https://www.python.org/downloads/release/python-388/)
+- [Python >=3.7](https://www.python.org/downloads/release/python-370/)
 
 # Licença
 
 [MIT](https://en.wikipedia.org/wiki/MIT_License)
```

