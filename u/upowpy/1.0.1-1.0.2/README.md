# Comparing `tmp/upowpy-1.0.1.tar.gz` & `tmp/upowpy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upowpy-1.0.1.tar", last modified: Wed May  1 08:35:16 2024, max compression
+gzip compressed data, was "upowpy-1.0.2.tar", last modified: Thu May  2 06:14:32 2024, max compression
```

## Comparing `upowpy-1.0.1.tar` & `upowpy-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 08:35:16.771404 upowpy-1.0.1/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     3807 2024-05-01 08:35:16.771153 upowpy-1.0.1/PKG-INFO
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     2981 2024-05-01 08:34:30.000000 upowpy-1.0.1/README.md
--rw-r--r--   0 georgeprethesh   (501) staff       (20)       38 2024-05-01 08:35:16.771450 upowpy-1.0.1/setup.cfg
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      986 2024-05-01 08:33:10.000000 upowpy-1.0.1/setup.py
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 08:35:16.766751 upowpy-1.0.1/upowpy/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      516 2024-05-01 07:29:26.000000 upowpy-1.0.1/upowpy/__init__.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     5080 2024-05-01 07:53:20.000000 upowpy-1.0.1/upowpy/push.py
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 08:35:16.769671 upowpy-1.0.1/upowpy/upow_transactions/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:21:00.000000 upowpy-1.0.1/upowpy/upow_transactions/__init__.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     1441 2024-05-01 07:35:56.000000 upowpy-1.0.1/upowpy/upow_transactions/coinbase_transaction.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      211 2024-03-01 05:05:06.000000 upowpy-1.0.1/upowpy/upow_transactions/constants.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     5524 2024-03-10 06:13:43.000000 upowpy-1.0.1/upowpy/upow_transactions/helpers.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     8573 2024-05-01 07:36:55.000000 upowpy-1.0.1/upowpy/upow_transactions/transaction.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     4945 2024-05-01 07:36:18.000000 upowpy-1.0.1/upowpy/upow_transactions/transaction_input.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     1522 2024-05-01 07:36:30.000000 upowpy-1.0.1/upowpy/upow_transactions/transaction_output.py
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 08:35:16.770572 upowpy-1.0.1/upowpy/utils/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:21:03.000000 upowpy-1.0.1/upowpy/utils/__init__.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)    17563 2024-05-01 07:48:39.000000 upowpy-1.0.1/upowpy/utils/repository.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)    22637 2024-05-01 07:48:08.000000 upowpy-1.0.1/upowpy/utils/utils.py
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 08:35:16.770856 upowpy-1.0.1/upowpy.egg-info/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     3807 2024-05-01 08:35:16.000000 upowpy-1.0.1/upowpy.egg-info/PKG-INFO
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      568 2024-05-01 08:35:16.000000 upowpy-1.0.1/upowpy.egg-info/SOURCES.txt
--rw-r--r--   0 georgeprethesh   (501) staff       (20)        1 2024-05-01 08:35:16.000000 upowpy-1.0.1/upowpy.egg-info/dependency_links.txt
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      233 2024-05-01 08:35:16.000000 upowpy-1.0.1/upowpy.egg-info/requires.txt
--rw-r--r--   0 georgeprethesh   (501) staff       (20)        7 2024-05-01 08:35:16.000000 upowpy-1.0.1/upowpy.egg-info/top_level.txt
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-02 06:14:32.755410 upowpy-1.0.2/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     3807 2024-05-02 06:14:32.755153 upowpy-1.0.2/PKG-INFO
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     2981 2024-05-01 08:34:30.000000 upowpy-1.0.2/README.md
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)       38 2024-05-02 06:14:32.755454 upowpy-1.0.2/setup.cfg
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      986 2024-05-02 06:14:00.000000 upowpy-1.0.2/setup.py
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-02 06:14:32.750753 upowpy-1.0.2/upowpy/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      516 2024-05-01 07:29:26.000000 upowpy-1.0.2/upowpy/__init__.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     4696 2024-05-02 06:13:22.000000 upowpy-1.0.2/upowpy/push.py
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-02 06:14:32.753537 upowpy-1.0.2/upowpy/upow_transactions/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:21:00.000000 upowpy-1.0.2/upowpy/upow_transactions/__init__.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     1441 2024-05-01 07:35:56.000000 upowpy-1.0.2/upowpy/upow_transactions/coinbase_transaction.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      211 2024-03-01 05:05:06.000000 upowpy-1.0.2/upowpy/upow_transactions/constants.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     5524 2024-03-10 06:13:43.000000 upowpy-1.0.2/upowpy/upow_transactions/helpers.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     8573 2024-05-01 07:36:55.000000 upowpy-1.0.2/upowpy/upow_transactions/transaction.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     4945 2024-05-01 07:36:18.000000 upowpy-1.0.2/upowpy/upow_transactions/transaction_input.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     1522 2024-05-01 07:36:30.000000 upowpy-1.0.2/upowpy/upow_transactions/transaction_output.py
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-02 06:14:32.754547 upowpy-1.0.2/upowpy/utils/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:21:03.000000 upowpy-1.0.2/upowpy/utils/__init__.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)    17563 2024-05-01 07:48:39.000000 upowpy-1.0.2/upowpy/utils/repository.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)    22637 2024-05-01 07:48:08.000000 upowpy-1.0.2/upowpy/utils/utils.py
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-02 06:14:32.754853 upowpy-1.0.2/upowpy.egg-info/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     3807 2024-05-02 06:14:32.000000 upowpy-1.0.2/upowpy.egg-info/PKG-INFO
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      568 2024-05-02 06:14:32.000000 upowpy-1.0.2/upowpy.egg-info/SOURCES.txt
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)        1 2024-05-02 06:14:32.000000 upowpy-1.0.2/upowpy.egg-info/dependency_links.txt
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      233 2024-05-02 06:14:32.000000 upowpy-1.0.2/upowpy.egg-info/requires.txt
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)        7 2024-05-02 06:14:32.000000 upowpy-1.0.2/upowpy.egg-info/top_level.txt
```

### Comparing `upowpy-1.0.1/PKG-INFO` & `upowpy-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upowpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: upowpy is a Python library for interacting with uPow blockchain transactions, including sending funds, staking, voting, and managing nodes and validators on the blockchain
 Home-page: https://github.com/upowai/upowpy
 Author: upow
 Author-email: contact@upow.ai
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: asttokens==2.4.1
```

### Comparing `upowpy-1.0.1/README.md` & `upowpy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.1/setup.py` & `upowpy-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="upowpy",
-    version="1.0.1",
+    version="1.0.2",
     author="upow",
     author_email="contact@upow.ai",
     description="upowpy is a Python library for interacting with uPow blockchain transactions, including sending funds, staking, voting, and managing nodes and validators on the blockchain",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/upowai/upowpy",
     packages=find_packages(),
```

### Comparing `upowpy-1.0.1/upowpy/__init__.py` & `upowpy-1.0.2/upowpy/__init__.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.1/upowpy/push.py` & `upowpy-1.0.2/upowpy/push.py`

 * *Files 16% similar despite different names*

```diff
@@ -55,71 +55,71 @@
         tx = await wallet_utils.create_stake_transaction(private_key, amount)
         error_message, transaction_hash = await push_tx(tx, wallet_utils)
         if transaction_hash:
             return transaction_hash
         else:
             raise Exception(error_message)
     except Exception as e:
-        logging.error(f"Error during staking transaction: {e}")
-        raise e
+
+        raise
 
 
 async def unstake_transaction(private_key_hex):
     try:
         private_key = int(private_key_hex, 16)
         tx = await wallet_utils.create_unstake_transaction(private_key)
         error_message, transaction_hash = await push_tx(tx, wallet_utils)
         if transaction_hash:
             return transaction_hash
         else:
             raise Exception(error_message)
     except Exception as e:
-        logging.error(f"Failed to unstake: {e}")
+
         raise
 
 
 async def register_inode_transaction(private_key_hex):
     try:
         private_key = int(private_key_hex, 16)
         tx = await wallet_utils.create_inode_registration_transaction(private_key)
         error_message, transaction_hash = await push_tx(tx, wallet_utils)
         if transaction_hash:
             return transaction_hash
         else:
             raise Exception(error_message)
     except Exception as e:
-        logging.error(f"Failed to register inode: {e}")
+
         raise
 
 
 async def deregister_inode_transaction(private_key_hex):
     try:
         private_key = int(private_key_hex, 16)
         tx = await wallet_utils.create_inode_de_registration_transaction(private_key)
         error_message, transaction_hash = await push_tx(tx, wallet_utils)
         if transaction_hash:
             return transaction_hash
         else:
             raise Exception(error_message)
     except Exception as e:
-        logging.error(f"Failed to deregister inode: {e}")
+
         raise
 
 
 async def register_validator_transaction(private_key_hex):
     try:
         private_key = int(private_key_hex, 16)
         tx = await wallet_utils.create_validator_registration_transaction(private_key)
         error_message, transaction_hash = await push_tx(tx, wallet_utils)
         if transaction_hash:
             return transaction_hash
         else:
             raise Exception(error_message)
     except Exception as e:
-        logging.error(f"Failed to register validator: {e}")
+
         raise
 
 
 async def vote_transaction(private_key_hex, voting_range, recipient):
     try:
         private_key = int(private_key_hex, 16)
         tx = await wallet_utils.create_voting_transaction(
@@ -127,23 +127,23 @@
         )
         error_message, transaction_hash = await push_tx(tx, wallet_utils)
         if transaction_hash:
             return transaction_hash
         else:
             raise Exception(error_message)
     except Exception as e:
-        logging.error(f"Failed to process vote: {e}")
+
         raise
 
 
 async def revoke_transaction(private_key_hex, revoke_from):
     try:
         private_key = int(private_key_hex, 16)
         tx = await wallet_utils.create_revoke_transaction(private_key, revoke_from)
         error_message, transaction_hash = await push_tx(tx, wallet_utils)
         if transaction_hash:
             return transaction_hash
         else:
             raise Exception(error_message)
     except Exception as e:
-        logging.error(f"Failed to revoke: {e}")
+
         raise
```

### Comparing `upowpy-1.0.1/upowpy/upow_transactions/coinbase_transaction.py` & `upowpy-1.0.2/upowpy/upow_transactions/coinbase_transaction.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.1/upowpy/upow_transactions/helpers.py` & `upowpy-1.0.2/upowpy/upow_transactions/helpers.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.1/upowpy/upow_transactions/transaction.py` & `upowpy-1.0.2/upowpy/upow_transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.1/upowpy/upow_transactions/transaction_input.py` & `upowpy-1.0.2/upowpy/upow_transactions/transaction_input.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.1/upowpy/upow_transactions/transaction_output.py` & `upowpy-1.0.2/upowpy/upow_transactions/transaction_output.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.1/upowpy/utils/repository.py` & `upowpy-1.0.2/upowpy/utils/repository.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.1/upowpy/utils/utils.py` & `upowpy-1.0.2/upowpy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.1/upowpy.egg-info/PKG-INFO` & `upowpy-1.0.2/upowpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upowpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: upowpy is a Python library for interacting with uPow blockchain transactions, including sending funds, staking, voting, and managing nodes and validators on the blockchain
 Home-page: https://github.com/upowai/upowpy
 Author: upow
 Author-email: contact@upow.ai
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: asttokens==2.4.1
```

### Comparing `upowpy-1.0.1/upowpy.egg-info/SOURCES.txt` & `upowpy-1.0.2/upowpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

