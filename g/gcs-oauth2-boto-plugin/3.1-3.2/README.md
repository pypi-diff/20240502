# Comparing `tmp/gcs-oauth2-boto-plugin-3.1.tar.gz` & `tmp/gcs-oauth2-boto-plugin-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcs-oauth2-boto-plugin-3.1.tar", last modified: Tue Apr 30 15:32:50 2024, max compression
+gzip compressed data, was "gcs-oauth2-boto-plugin-3.2.tar", last modified: Thu May  2 14:37:30 2024, max compression
```

## Comparing `gcs-oauth2-boto-plugin-3.1.tar` & `gcs-oauth2-boto-plugin-3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 margubur (1016367) primarygroup (89939)        0 2024-04-30 15:32:50.186235 gcs-oauth2-boto-plugin-3.1/
--rw-r--r--   0 margubur (1016367) primarygroup (89939)    11359 2024-04-30 09:50:35.000000 gcs-oauth2-boto-plugin-3.1/LICENSE
--rw-r--r--   0 margubur (1016367) primarygroup (89939)       16 2024-04-30 09:50:35.000000 gcs-oauth2-boto-plugin-3.1/MANIFEST.in
--rw-r--r--   0 margubur (1016367) primarygroup (89939)     1506 2024-04-30 15:32:50.186235 gcs-oauth2-boto-plugin-3.1/PKG-INFO
--rw-r--r--   0 margubur (1016367) primarygroup (89939)     2222 2024-04-30 09:50:35.000000 gcs-oauth2-boto-plugin-3.1/README.md
-drwxr-xr-x   0 margubur (1016367) primarygroup (89939)        0 2024-04-30 15:32:50.182235 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/
--rw-r--r--   0 margubur (1016367) primarygroup (89939)     1542 2024-04-30 09:50:35.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/__init__.py
--rw-r--r--   0 margubur (1016367) primarygroup (89939)    32344 2024-04-30 09:50:35.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/oauth2_client.py
--rw-r--r--   0 margubur (1016367) primarygroup (89939)     8540 2024-04-30 09:50:35.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/oauth2_helper.py
--rw-r--r--   0 margubur (1016367) primarygroup (89939)     2736 2024-04-30 09:50:35.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/oauth2_plugin.py
--rw-r--r--   0 margubur (1016367) primarygroup (89939)    14135 2024-04-30 09:50:35.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/test_oauth2_client.py
-drwxr-xr-x   0 margubur (1016367) primarygroup (89939)        0 2024-04-30 15:32:50.186235 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin.egg-info/
--rw-r--r--   0 margubur (1016367) primarygroup (89939)     1506 2024-04-30 15:32:50.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin.egg-info/PKG-INFO
--rw-r--r--   0 margubur (1016367) primarygroup (89939)      518 2024-04-30 15:32:50.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 margubur (1016367) primarygroup (89939)        1 2024-04-30 15:32:50.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 margubur (1016367) primarygroup (89939)      183 2024-04-30 15:32:50.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin.egg-info/requires.txt
--rw-r--r--   0 margubur (1016367) primarygroup (89939)       23 2024-04-30 15:32:50.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin.egg-info/top_level.txt
--rw-r--r--   0 margubur (1016367) primarygroup (89939)        1 2024-04-30 15:32:50.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin.egg-info/zip-safe
--rw-r--r--   0 margubur (1016367) primarygroup (89939)       74 2024-04-30 15:32:50.186235 gcs-oauth2-boto-plugin-3.1/setup.cfg
--rw-r--r--   0 margubur (1016367) primarygroup (89939)     2935 2024-04-30 09:50:35.000000 gcs-oauth2-boto-plugin-3.1/setup.py
+drwxr-xr-x   0 margubur (1016367) primarygroup (89939)        0 2024-05-02 14:37:30.734307 gcs-oauth2-boto-plugin-3.2/
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)    11359 2024-05-02 14:35:25.000000 gcs-oauth2-boto-plugin-3.2/LICENSE
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)       16 2024-05-02 14:35:25.000000 gcs-oauth2-boto-plugin-3.2/MANIFEST.in
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)     1506 2024-05-02 14:37:30.734307 gcs-oauth2-boto-plugin-3.2/PKG-INFO
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)     2222 2024-05-02 14:35:25.000000 gcs-oauth2-boto-plugin-3.2/README.md
+drwxr-xr-x   0 margubur (1016367) primarygroup (89939)        0 2024-05-02 14:37:30.730307 gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin/
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)     1542 2024-05-02 14:35:25.000000 gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin/__init__.py
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)    32344 2024-05-02 14:35:25.000000 gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin/oauth2_client.py
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)     8540 2024-05-02 14:35:25.000000 gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin/oauth2_helper.py
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)     2736 2024-05-02 14:35:25.000000 gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin/oauth2_plugin.py
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)    14135 2024-05-02 14:35:25.000000 gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin/test_oauth2_client.py
+drwxr-xr-x   0 margubur (1016367) primarygroup (89939)        0 2024-05-02 14:37:30.734307 gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin.egg-info/
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)     1506 2024-05-02 14:37:30.000000 gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)      518 2024-05-02 14:37:30.000000 gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)        1 2024-05-02 14:37:30.000000 gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)      231 2024-05-02 14:37:30.000000 gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin.egg-info/requires.txt
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)       23 2024-05-02 14:37:30.000000 gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin.egg-info/top_level.txt
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)        1 2024-05-02 14:37:30.000000 gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin.egg-info/zip-safe
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)       74 2024-05-02 14:37:30.734307 gcs-oauth2-boto-plugin-3.2/setup.cfg
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)     2997 2024-05-02 14:35:25.000000 gcs-oauth2-boto-plugin-3.2/setup.py
```

### Comparing `gcs-oauth2-boto-plugin-3.1/LICENSE` & `gcs-oauth2-boto-plugin-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gcs-oauth2-boto-plugin-3.1/PKG-INFO` & `gcs-oauth2-boto-plugin-3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcs-oauth2-boto-plugin
-Version: 3.1
+Version: 3.2
 Summary: Auth plugin allowing use the use of OAuth 2.0 credentials for Google Cloud Storage in the Boto library.
 Home-page: https://developers.google.com/storage/docs/gspythonlibrary
 Download-URL: https://github.com/GoogleCloudPlatform/gcs-oauth2-boto-plugin
 Author: Google Inc.
 Author-email: gs-team@google.com
 License: Apache 2.0
 Platform: any
```

### Comparing `gcs-oauth2-boto-plugin-3.1/README.md` & `gcs-oauth2-boto-plugin-3.2/README.md`

 * *Files identical despite different names*

### Comparing `gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/__init__.py` & `gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/oauth2_client.py` & `gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin/oauth2_client.py`

 * *Files identical despite different names*

### Comparing `gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/oauth2_helper.py` & `gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin/oauth2_helper.py`

 * *Files identical despite different names*

### Comparing `gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/oauth2_plugin.py` & `gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin/oauth2_plugin.py`

 * *Files identical despite different names*

### Comparing `gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/test_oauth2_client.py` & `gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin/test_oauth2_client.py`

 * *Files identical despite different names*

### Comparing `gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin.egg-info/PKG-INFO` & `gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcs-oauth2-boto-plugin
-Version: 3.1
+Version: 3.2
 Summary: Auth plugin allowing use the use of OAuth 2.0 credentials for Google Cloud Storage in the Boto library.
 Home-page: https://developers.google.com/storage/docs/gspythonlibrary
 Download-URL: https://github.com/GoogleCloudPlatform/gcs-oauth2-boto-plugin
 Author: Google Inc.
 Author-email: gs-team@google.com
 License: Apache 2.0
 Platform: any
```

### Comparing `gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin.egg-info/SOURCES.txt` & `gcs-oauth2-boto-plugin-3.2/gcs_oauth2_boto_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcs-oauth2-boto-plugin-3.1/setup.py` & `gcs-oauth2-boto-plugin-3.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,27 +32,29 @@
     'rsa==4.7.2',
     'boto>=2.29.1',
     'google-reauth>=0.1.0',
     'httplib2>=0.18',
     'oauth2client>=2.2.0',
     'pyOpenSSL>=0.13',
     'retry_decorator>=1.0.0',
-    'six>=1.12.0'
+    'six>=1.12.0',
+    'google-auth==2.17.0',
+    'google-auth-httplib2>=0.2.0'
 ]
 
 extras_require = {
     'dev': [
         'freezegun',
         'mock;python_version<"3.3"',
     ],
 }
 
 setup(
     name='gcs-oauth2-boto-plugin',
-    version='3.1',
+    version='3.2',
     url='https://developers.google.com/storage/docs/gspythonlibrary',
     download_url=('https://github.com/GoogleCloudPlatform'
                   '/gcs-oauth2-boto-plugin'),
     license='Apache 2.0',
     author='Google Inc.',
     author_email='gs-team@google.com',
     description=('Auth plugin allowing use the use of OAuth 2.0 credentials '
```

