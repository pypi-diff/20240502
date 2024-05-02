# Comparing `tmp/amazon_sdk-0.0.5.tar.gz` & `tmp/amazon_sdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon_sdk-0.0.5.tar", max compression
+gzip compressed data, was "amazon_sdk-0.0.6.tar", max compression
```

## Comparing `amazon_sdk-0.0.5.tar` & `amazon_sdk-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       71 2024-05-02 15:34:46.656945 amazon_sdk-0.0.5/Amazon_SDK/__init__.py
--rw-r--r--   0        0        0     7731 2024-05-02 16:05:53.533879 amazon_sdk-0.0.5/Amazon_SDK/amz_sdk.py
--rw-r--r--   0        0        0      780 2024-04-29 13:08:42.565891 amazon_sdk-0.0.5/Amazon_SDK/order_statuses.py
--rw-r--r--   0        0        0      302 2024-05-02 16:10:14.927731 amazon_sdk-0.0.5/README.md
--rw-r--r--   0        0        0      387 2024-05-02 16:40:23.705729 amazon_sdk-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 amazon_sdk-0.0.5/setup.py
--rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 amazon_sdk-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       71 2024-05-02 15:34:46.656945 amazon_sdk-0.0.6/Amazon_SDK/__init__.py
+-rw-r--r--   0        0        0     7882 2024-05-02 17:23:29.937181 amazon_sdk-0.0.6/Amazon_SDK/amz_sdk.py
+-rw-r--r--   0        0        0      780 2024-04-29 13:08:42.565891 amazon_sdk-0.0.6/Amazon_SDK/order_statuses.py
+-rw-r--r--   0        0        0      497 2024-05-02 17:23:01.925727 amazon_sdk-0.0.6/README.md
+-rw-r--r--   0        0        0      387 2024-05-02 17:23:57.595963 amazon_sdk-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 amazon_sdk-0.0.6/setup.py
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 amazon_sdk-0.0.6/PKG-INFO
```

### Comparing `amazon_sdk-0.0.5/Amazon_SDK/amz_sdk.py` & `amazon_sdk-0.0.6/Amazon_SDK/amz_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from dotenv import load_dotenv
 
 from .order_statuses import OrderStatus, validate_order_status
 
 class AmazonSDK:
     # exported functions do not check params but check the returned status code
     def __init__(self, dotenv_path: str = None):
+        """
+        Initializes the AmazonSDK object with the given dotenv file path.
+        :param dotenv_path: path to the dotenv file.
+        """
         self.MARKETPLACE_IDS = ["A1805IZSGTT6HS"]
         self.ENDPOINT = "https://sellingpartnerapi-eu.amazon.com"
         # print 1+1
 
         # =============================================================================
         # Calling the API credentials:
         # ----------------------------
```

### Comparing `amazon_sdk-0.0.5/Amazon_SDK/order_statuses.py` & `amazon_sdk-0.0.6/Amazon_SDK/order_statuses.py`

 * *Files identical despite different names*

### Comparing `amazon_sdk-0.0.5/setup.py` & `amazon_sdk-0.0.6/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['python-dotenv>=1.0.1,<2.0.0', 'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'amazon-sdk',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': 'A package for Amazon SDK',
-    'long_description': '# Amazon SDK\n\n## Installation\n\n```bash\npip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps Amazon-SDK \n```\n\n## Usage\n\nDifferences with bol_sdk:\n- Use methods in class `AmazonSDK`, with detailed documentation\n- No need to pass the `access_token`\n\nFor example see `usage_example.py`',
+    'long_description': '# Amazon SDK\n\n## Setup\n\n1. Install the package:\n\n```bash\npip install --upgrade Amazon_SDK\n```\n\n2. Add file `.env` with the following content:\n\n```plaintext\nLWA_APP_ID=<your_app_id>\nLWA_CLIENT_SECRET=<your_client_secret>\nSP_API_REFRESH_TOKEN=<your_refresh_token>\n```\n\n## Usage\n\nFor example see `usage_example.py`\n\nDifferences with `bol_SDK`:\n- Use methods in class `AmazonSDK`, with detailed documentation\n- No need to pass `access_token` as a parameter, which is automatically handled by the SDK\n\n',
     'author': 'Genhao Li',
     'author_email': 'ligenhao20010916@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

