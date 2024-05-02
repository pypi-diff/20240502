# Comparing `tmp/uma_sdk-1.0.4.zip` & `tmp/uma_sdk-1.0.5.zip`

## zipinfo {}

```diff
@@ -1,49 +1,49 @@
-Zip file size: 39790 bytes, number of entries: 47
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 17:34 uma_sdk-1.0.4/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 17:34 uma_sdk-1.0.4/uma_sdk.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 17:34 uma_sdk-1.0.4/uma/
--rw-r--r--  2.0 unx    11352 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/LICENSE
--rwxr-xr-x  2.0 unx       87 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/setup.py
--rw-r--r--  2.0 unx      133 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/README.md
--rw-r--r--  2.0 unx       81 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/pyproject.toml
--rw-r--r--  2.0 unx      648 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/setup.cfg
--rw-r--r--  2.0 unx      631 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/PKG-INFO
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma_sdk.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx      924 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma_sdk.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma_sdk.egg-info/top_level.txt
--rw-r--r--  2.0 unx      631 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma_sdk.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       30 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma_sdk.egg-info/requires.txt
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/
--rw-r--r--  2.0 unx     3407 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/JSONable.py
--rw-r--r--  2.0 unx     1624 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/public_key_cache.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/py.typed
--rw-r--r--  2.0 unx      284 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/uma_invoice_creator.py
--rw-r--r--  2.0 unx     2878 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/version.py
--rw-r--r--  2.0 unx      239 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/type_utils.py
--rw-r--r--  2.0 unx     2061 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/nonce_cache.py
--rw-r--r--  2.0 unx     2160 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/__init__.py
--rw-r--r--  2.0 unx     1117 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/cert_utils.py
--rw-r--r--  2.0 unx      266 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/urls.py
--rw-r--r--  2.0 unx    30711 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/uma.py
--rw-r--r--  2.0 unx      868 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/exceptions.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/v1/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/v0/
--rw-r--r--  2.0 unx     2591 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/lnurlp_request.py
--rw-r--r--  2.0 unx     8829 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/payreq_response.py
--rw-r--r--  2.0 unx     1724 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/post_tx_callback.py
--rw-r--r--  2.0 unx      132 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/payee_data.py
--rw-r--r--  2.0 unx     2307 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/payer_data.py
--rw-r--r--  2.0 unx      557 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/counterparty_data.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/__init__.py
--rw-r--r--  2.0 unx     3324 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/lnurlp_response.py
--rw-r--r--  2.0 unx     6328 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/payreq.py
--rw-r--r--  2.0 unx     4498 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/pubkey_response.py
--rw-r--r--  2.0 unx     4609 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/currency.py
--rw-r--r--  2.0 unx      231 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/kyc_status.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/v1/__init__.py
--rw-r--r--  2.0 unx     4294 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/v1/payreq.py
--rw-r--r--  2.0 unx     2702 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/v1/currency.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/v0/__init__.py
--rw-r--r--  2.0 unx     1788 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/v0/payreq.py
--rw-r--r--  2.0 unx     1950 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/v0/currency.py
-47 files, 106001 bytes uncompressed, 32962 bytes compressed:  68.9%
+Zip file size: 40084 bytes, number of entries: 47
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 21:08 uma_sdk-1.0.5/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 21:08 uma_sdk-1.0.5/uma_sdk.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 21:08 uma_sdk-1.0.5/uma/
+-rw-r--r--  2.0 unx    11352 b- defN 24-May-02 21:08 uma_sdk-1.0.5/LICENSE
+-rwxr-xr-x  2.0 unx       87 b- defN 24-May-02 21:08 uma_sdk-1.0.5/setup.py
+-rw-r--r--  2.0 unx      133 b- defN 24-May-02 21:08 uma_sdk-1.0.5/README.md
+-rw-r--r--  2.0 unx       81 b- defN 24-May-02 21:08 uma_sdk-1.0.5/pyproject.toml
+-rw-r--r--  2.0 unx      648 b- defN 24-May-02 21:08 uma_sdk-1.0.5/setup.cfg
+-rw-r--r--  2.0 unx      631 b- defN 24-May-02 21:08 uma_sdk-1.0.5/PKG-INFO
+-rw-r--r--  2.0 unx        1 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma_sdk.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx      924 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma_sdk.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma_sdk.egg-info/top_level.txt
+-rw-r--r--  2.0 unx      631 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma_sdk.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       30 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma_sdk.egg-info/requires.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/
+-rw-r--r--  2.0 unx     3407 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/JSONable.py
+-rw-r--r--  2.0 unx     1624 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/public_key_cache.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/py.typed
+-rw-r--r--  2.0 unx      284 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/uma_invoice_creator.py
+-rw-r--r--  2.0 unx     2878 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/version.py
+-rw-r--r--  2.0 unx      239 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/type_utils.py
+-rw-r--r--  2.0 unx     2061 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/nonce_cache.py
+-rw-r--r--  2.0 unx     2160 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/__init__.py
+-rw-r--r--  2.0 unx     1117 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/cert_utils.py
+-rw-r--r--  2.0 unx      266 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/urls.py
+-rw-r--r--  2.0 unx    30711 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/uma.py
+-rw-r--r--  2.0 unx      868 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/exceptions.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/v1/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/v0/
+-rw-r--r--  2.0 unx     2591 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/lnurlp_request.py
+-rw-r--r--  2.0 unx     8829 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/payreq_response.py
+-rw-r--r--  2.0 unx     1724 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/post_tx_callback.py
+-rw-r--r--  2.0 unx      132 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/payee_data.py
+-rw-r--r--  2.0 unx     2307 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/payer_data.py
+-rw-r--r--  2.0 unx      557 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/counterparty_data.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/__init__.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/lnurlp_response.py
+-rw-r--r--  2.0 unx     7993 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/payreq.py
+-rw-r--r--  2.0 unx     4498 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/pubkey_response.py
+-rw-r--r--  2.0 unx     4609 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/currency.py
+-rw-r--r--  2.0 unx      231 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/kyc_status.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/v1/__init__.py
+-rw-r--r--  2.0 unx     4294 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/v1/payreq.py
+-rw-r--r--  2.0 unx     2702 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/v1/currency.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/v0/__init__.py
+-rw-r--r--  2.0 unx     1788 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/v0/payreq.py
+-rw-r--r--  2.0 unx     1950 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/v0/currency.py
+47 files, 107666 bytes uncompressed, 33256 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -1,142 +1,142 @@
-Filename: uma_sdk-1.0.4/
+Filename: uma_sdk-1.0.5/
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma_sdk.egg-info/
+Filename: uma_sdk-1.0.5/uma_sdk.egg-info/
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/
+Filename: uma_sdk-1.0.5/uma/
 Comment: 
 
-Filename: uma_sdk-1.0.4/LICENSE
+Filename: uma_sdk-1.0.5/LICENSE
 Comment: 
 
-Filename: uma_sdk-1.0.4/setup.py
+Filename: uma_sdk-1.0.5/setup.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/README.md
+Filename: uma_sdk-1.0.5/README.md
 Comment: 
 
-Filename: uma_sdk-1.0.4/pyproject.toml
+Filename: uma_sdk-1.0.5/pyproject.toml
 Comment: 
 
-Filename: uma_sdk-1.0.4/setup.cfg
+Filename: uma_sdk-1.0.5/setup.cfg
 Comment: 
 
-Filename: uma_sdk-1.0.4/PKG-INFO
+Filename: uma_sdk-1.0.5/PKG-INFO
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma_sdk.egg-info/dependency_links.txt
+Filename: uma_sdk-1.0.5/uma_sdk.egg-info/dependency_links.txt
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma_sdk.egg-info/SOURCES.txt
+Filename: uma_sdk-1.0.5/uma_sdk.egg-info/SOURCES.txt
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma_sdk.egg-info/top_level.txt
+Filename: uma_sdk-1.0.5/uma_sdk.egg-info/top_level.txt
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma_sdk.egg-info/PKG-INFO
+Filename: uma_sdk-1.0.5/uma_sdk.egg-info/PKG-INFO
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma_sdk.egg-info/requires.txt
+Filename: uma_sdk-1.0.5/uma_sdk.egg-info/requires.txt
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/
+Filename: uma_sdk-1.0.5/uma/protocol/
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/JSONable.py
+Filename: uma_sdk-1.0.5/uma/JSONable.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/public_key_cache.py
+Filename: uma_sdk-1.0.5/uma/public_key_cache.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/py.typed
+Filename: uma_sdk-1.0.5/uma/py.typed
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/uma_invoice_creator.py
+Filename: uma_sdk-1.0.5/uma/uma_invoice_creator.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/version.py
+Filename: uma_sdk-1.0.5/uma/version.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/type_utils.py
+Filename: uma_sdk-1.0.5/uma/type_utils.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/nonce_cache.py
+Filename: uma_sdk-1.0.5/uma/nonce_cache.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/__init__.py
+Filename: uma_sdk-1.0.5/uma/__init__.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/cert_utils.py
+Filename: uma_sdk-1.0.5/uma/cert_utils.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/urls.py
+Filename: uma_sdk-1.0.5/uma/urls.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/uma.py
+Filename: uma_sdk-1.0.5/uma/uma.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/exceptions.py
+Filename: uma_sdk-1.0.5/uma/exceptions.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/v1/
+Filename: uma_sdk-1.0.5/uma/protocol/v1/
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/v0/
+Filename: uma_sdk-1.0.5/uma/protocol/v0/
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/lnurlp_request.py
+Filename: uma_sdk-1.0.5/uma/protocol/lnurlp_request.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/payreq_response.py
+Filename: uma_sdk-1.0.5/uma/protocol/payreq_response.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/post_tx_callback.py
+Filename: uma_sdk-1.0.5/uma/protocol/post_tx_callback.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/payee_data.py
+Filename: uma_sdk-1.0.5/uma/protocol/payee_data.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/payer_data.py
+Filename: uma_sdk-1.0.5/uma/protocol/payer_data.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/counterparty_data.py
+Filename: uma_sdk-1.0.5/uma/protocol/counterparty_data.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/__init__.py
+Filename: uma_sdk-1.0.5/uma/protocol/__init__.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/lnurlp_response.py
+Filename: uma_sdk-1.0.5/uma/protocol/lnurlp_response.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/payreq.py
+Filename: uma_sdk-1.0.5/uma/protocol/payreq.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/pubkey_response.py
+Filename: uma_sdk-1.0.5/uma/protocol/pubkey_response.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/currency.py
+Filename: uma_sdk-1.0.5/uma/protocol/currency.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/kyc_status.py
+Filename: uma_sdk-1.0.5/uma/protocol/kyc_status.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/v1/__init__.py
+Filename: uma_sdk-1.0.5/uma/protocol/v1/__init__.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/v1/payreq.py
+Filename: uma_sdk-1.0.5/uma/protocol/v1/payreq.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/v1/currency.py
+Filename: uma_sdk-1.0.5/uma/protocol/v1/currency.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/v0/__init__.py
+Filename: uma_sdk-1.0.5/uma/protocol/v0/__init__.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/v0/payreq.py
+Filename: uma_sdk-1.0.5/uma/protocol/v0/payreq.py
 Comment: 
 
-Filename: uma_sdk-1.0.4/uma/protocol/v0/currency.py
+Filename: uma_sdk-1.0.5/uma/protocol/v0/currency.py
 Comment: 
 
 Zip file comment:
```

## Comparing `uma_sdk-1.0.4/LICENSE` & `uma_sdk-1.0.5/LICENSE`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/setup.cfg` & `uma_sdk-1.0.5/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = uma-sdk
-version = 1.0.4
+version = 1.0.5
 description = Python SDK for UMA (universal money address)
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Lightspark Group, Inc.
 author_email = info@lightspark.com
 license = Apache-2.0
 license_files = LICENSE
```

## Comparing `uma_sdk-1.0.4/PKG-INFO` & `uma_sdk-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uma-sdk
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python SDK for UMA (universal money address)
 Author: Lightspark Group, Inc.
 Author-email: info@lightspark.com
 License: Apache-2.0
 Project-URL: Documentation, https://app.lightspark.com/docs/uma-sdk/introduction
 Project-URL: Source Code, https://github.com/uma-universal-money-address/uma-python-sdk/
 Description-Content-Type: text/markdown
```

## Comparing `uma_sdk-1.0.4/uma_sdk.egg-info/SOURCES.txt` & `uma_sdk-1.0.5/uma_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma_sdk.egg-info/PKG-INFO` & `uma_sdk-1.0.5/uma_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uma-sdk
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python SDK for UMA (universal money address)
 Author: Lightspark Group, Inc.
 Author-email: info@lightspark.com
 License: Apache-2.0
 Project-URL: Documentation, https://app.lightspark.com/docs/uma-sdk/introduction
 Project-URL: Source Code, https://github.com/uma-universal-money-address/uma-python-sdk/
 Description-Content-Type: text/markdown
```

## Comparing `uma_sdk-1.0.4/uma/JSONable.py` & `uma_sdk-1.0.5/uma/JSONable.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/public_key_cache.py` & `uma_sdk-1.0.5/uma/public_key_cache.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/version.py` & `uma_sdk-1.0.5/uma/version.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/nonce_cache.py` & `uma_sdk-1.0.5/uma/nonce_cache.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/__init__.py` & `uma_sdk-1.0.5/uma/__init__.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/cert_utils.py` & `uma_sdk-1.0.5/uma/cert_utils.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/uma.py` & `uma_sdk-1.0.5/uma/uma.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/exceptions.py` & `uma_sdk-1.0.5/uma/exceptions.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/protocol/lnurlp_request.py` & `uma_sdk-1.0.5/uma/protocol/lnurlp_request.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/protocol/payreq_response.py` & `uma_sdk-1.0.5/uma/protocol/payreq_response.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/protocol/post_tx_callback.py` & `uma_sdk-1.0.5/uma/protocol/post_tx_callback.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/protocol/payer_data.py` & `uma_sdk-1.0.5/uma/protocol/payer_data.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/protocol/counterparty_data.py` & `uma_sdk-1.0.5/uma/protocol/counterparty_data.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/protocol/lnurlp_response.py` & `uma_sdk-1.0.5/uma/protocol/lnurlp_response.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/protocol/payreq.py` & `uma_sdk-1.0.5/uma/protocol/payreq.py`

 * *Files 13% similar despite different names*

```diff
@@ -114,16 +114,16 @@
 
     @classmethod
     def from_json(cls: "type[PayRequest]", json_encoded: str) -> "PayRequest":
         json_dict = json.loads(json_encoded)
         is_amount_string = "amount" in json_dict and isinstance(
             json_dict["amount"], str
         )
-        is_uma = "payerData" in json_dict and "compliance" in json_dict["payerData"]
-        is_v1 = ("convert" in json_dict) and is_uma
+        is_uma = json_dict.get("payerData") and "compliance" in json_dict["payerData"]
+        is_v1 = "convert" in json_dict and is_uma
         is_v0 = "currency" in json_dict and is_uma
 
         if is_v1 or is_amount_string:
             v1_payreq = V1PayRequest.from_json(json_encoded)
             return PayRequest(
                 sending_amount_currency_code=v1_payreq.sending_amount_currency_code,
                 receiving_currency_code=v1_payreq.receiving_currency_code,
@@ -138,7 +138,46 @@
             sending_amount_currency_code=v0_payreq.currency_code,
             receiving_currency_code=v0_payreq.currency_code,
             amount=v0_payreq.amount,
             payer_data=v0_payreq.payer_data,
             requested_payee_data=None,
             uma_major_version=0 if is_v0 else None,
         )
+
+    def to_request_params(self) -> Dict[str, str]:
+        params = {}
+        if self.sending_amount_currency_code:
+            amount = f"{self.amount}.{self.sending_amount_currency_code}"
+        else:
+            amount = str(self.amount)
+        params["amount"] = amount
+        if self.receiving_currency_code:
+            params["convert"] = self.receiving_currency_code
+        if self.payer_data is not None:
+            params["payerData"] = json.dumps(self.payer_data)
+        if self.requested_payee_data is not None:
+            params["payeeData"] = json.dumps(self.requested_payee_data)
+        if self.comment:
+            params["comment"] = self.comment
+        return params
+
+    @classmethod
+    def from_request_params(
+        cls: "type[PayRequest]", params: Dict[str, str]
+    ) -> "PayRequest":
+        if not params.get("amount"):
+            raise InvalidRequestException("amount is required.")
+        parts = params["amount"].split(".")
+        sending_amount_currency_code = parts[1] if len(parts) == 2 else None
+        amount = parts[0]
+        payer_data_json = params.get("payerData")
+        payer_data = None if payer_data_json is None else json.loads(payer_data_json)
+        payee_data_json = params.get("payeeData")
+        payee_data = None if payee_data_json is None else json.loads(payee_data_json)
+        return PayRequest(
+            sending_amount_currency_code=sending_amount_currency_code,
+            receiving_currency_code=params.get("convert"),
+            amount=int(amount),
+            payer_data=payer_data,
+            comment=params.get("comment"),
+            requested_payee_data=payee_data,
+        )
```

## Comparing `uma_sdk-1.0.4/uma/protocol/pubkey_response.py` & `uma_sdk-1.0.5/uma/protocol/pubkey_response.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/protocol/currency.py` & `uma_sdk-1.0.5/uma/protocol/currency.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/protocol/v1/payreq.py` & `uma_sdk-1.0.5/uma/protocol/v1/payreq.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/protocol/v1/currency.py` & `uma_sdk-1.0.5/uma/protocol/v1/currency.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/protocol/v0/payreq.py` & `uma_sdk-1.0.5/uma/protocol/v0/payreq.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.4/uma/protocol/v0/currency.py` & `uma_sdk-1.0.5/uma/protocol/v0/currency.py`

 * *Files identical despite different names*

