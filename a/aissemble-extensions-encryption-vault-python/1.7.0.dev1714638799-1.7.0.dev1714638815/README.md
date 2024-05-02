# Comparing `tmp/aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799.tar.gz` & `tmp/aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799.tar", max compression
+gzip compressed data, was "aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815.tar", max compression
```

## Comparing `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799.tar` & `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     9580 2024-05-02 08:33:06.496278 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/LICENSE
--rw-r--r--   0        0        0     5089 2024-05-02 08:12:10.091802 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/README.md
--rw-r--r--   0        0        0      693 2024-05-02 08:33:20.121267 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/pyproject.toml
--rw-r--r--   0        0        0      205 2024-05-02 08:12:10.091802 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/__init__.py
--rw-r--r--   0        0        0     1939 2024-05-02 08:12:10.091802 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/aes_cbc_encrypt.py
--rw-r--r--   0        0        0      808 2024-05-02 08:12:10.091802 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/aes_cbc_encryption_strategy.py
--rw-r--r--   0        0        0     2243 2024-05-02 08:12:10.091802 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/aes_gcm_96_encrypt.py
--rw-r--r--   0        0        0      886 2024-05-02 08:12:10.091802 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/aes_gcm_96_encryption_strategy.py
--rw-r--r--   0        0        0      392 2024-05-02 08:12:10.091802 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/strategy_base.py
--rw-r--r--   0        0        0     2497 2024-05-02 08:12:10.091802 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/vault_config.py
--rw-r--r--   0        0        0     5131 2024-05-02 08:12:10.091802 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/vault_encrypt.py
--rw-r--r--   0        0        0     3818 2024-05-02 08:12:10.091802 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/vault_key_util.py
--rw-r--r--   0        0        0     1082 2024-05-02 08:12:10.091802 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/vault_local_encryption_strategy.py
--rw-r--r--   0        0        0      912 2024-05-02 08:12:10.091802 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/vault_remote_encryption_strategy.py
--rw-r--r--   0        0        0     5622 1970-01-01 00:00:00.000000 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-02 08:33:19.863485 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/LICENSE
+-rw-r--r--   0        0        0     5089 2024-05-02 08:12:10.898922 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/README.md
+-rw-r--r--   0        0        0      693 2024-05-02 08:33:36.073032 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/pyproject.toml
+-rw-r--r--   0        0        0      205 2024-05-02 08:12:10.898922 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/__init__.py
+-rw-r--r--   0        0        0     1939 2024-05-02 08:12:10.898922 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/aes_cbc_encrypt.py
+-rw-r--r--   0        0        0      808 2024-05-02 08:12:10.898922 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/aes_cbc_encryption_strategy.py
+-rw-r--r--   0        0        0     2243 2024-05-02 08:12:10.898922 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/aes_gcm_96_encrypt.py
+-rw-r--r--   0        0        0      886 2024-05-02 08:12:10.898922 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/aes_gcm_96_encryption_strategy.py
+-rw-r--r--   0        0        0      392 2024-05-02 08:12:10.898922 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/strategy_base.py
+-rw-r--r--   0        0        0     2497 2024-05-02 08:12:10.898922 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/vault_config.py
+-rw-r--r--   0        0        0     5131 2024-05-02 08:12:10.898922 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/vault_encrypt.py
+-rw-r--r--   0        0        0     3818 2024-05-02 08:12:10.898922 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/vault_key_util.py
+-rw-r--r--   0        0        0     1082 2024-05-02 08:12:10.898922 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/vault_local_encryption_strategy.py
+-rw-r--r--   0        0        0      912 2024-05-02 08:12:10.898922 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/vault_remote_encryption_strategy.py
+-rw-r--r--   0        0        0     5622 1970-01-01 00:00:00.000000 aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/PKG-INFO
```

### Comparing `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/LICENSE` & `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/README.md` & `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/README.md`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/pyproject.toml` & `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-extensions-encryption-vault-python"
-version = "1.7.0.dev1714638799"
+version = "1.7.0.dev1714638815"
 description = "Vault data encryption classes (python)"
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "aiops_encrypt", from="src"}
 ]
```

### Comparing `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/aes_cbc_encrypt.py` & `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/aes_cbc_encrypt.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/aes_cbc_encryption_strategy.py` & `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/aes_cbc_encryption_strategy.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/aes_gcm_96_encrypt.py` & `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/aes_gcm_96_encrypt.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/aes_gcm_96_encryption_strategy.py` & `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/aes_gcm_96_encryption_strategy.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/vault_config.py` & `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/vault_config.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/vault_encrypt.py` & `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/vault_encrypt.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/vault_key_util.py` & `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/vault_key_util.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/vault_local_encryption_strategy.py` & `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/vault_local_encryption_strategy.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/src/aiops_encrypt/vault_remote_encryption_strategy.py` & `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/src/aiops_encrypt/vault_remote_encryption_strategy.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638799/PKG-INFO` & `aissemble_extensions_encryption_vault_python-1.7.0.dev1714638815/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-extensions-encryption-vault-python
-Version: 1.7.0.dev1714638799
+Version: 1.7.0.dev1714638815
 Summary: Vault data encryption classes (python)
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cryptography (>=42.0.4)
```

