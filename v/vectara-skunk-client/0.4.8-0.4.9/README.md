# Comparing `tmp/vectara-skunk-client-0.4.8.tar.gz` & `tmp/vectara-skunk-client-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectara-skunk-client-0.4.8.tar", last modified: Fri Jan 12 21:27:24 2024, max compression
+gzip compressed data, was "vectara-skunk-client-0.4.9.tar", last modified: Fri Jan 12 21:39:23 2024, max compression
```

## Comparing `vectara-skunk-client-0.4.8.tar` & `vectara-skunk-client-0.4.9.tar`

### file list

```diff
@@ -1,27 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-01-12 21:27:24.467467 vectara-skunk-client-0.4.8/
--rw-rw-rw-   0        0        0    34918 2023-12-21 21:26:20.000000 vectara-skunk-client-0.4.8/LICENSE.md
--rw-rw-rw-   0        0        0      911 2024-01-12 21:27:24.466405 vectara-skunk-client-0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     5222 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.8/README.md
--rw-rw-rw-   0        0        0       42 2024-01-12 21:27:24.468537 vectara-skunk-client-0.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1372 2024-01-12 21:23:13.000000 vectara-skunk-client-0.4.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-12 21:27:24.445337 vectara-skunk-client-0.4.8/test/
--rw-rw-rw-   0        0        0     5280 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.8/test/test_api_keys.py
--rw-rw-rw-   0        0        0     2400 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.8/test/test_arabic.py
--rw-rw-rw-   0        0        0     1348 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.8/test/test_basic_query.py
--rw-rw-rw-   0        0        0     1395 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.8/test/test_documents.py
--rw-rw-rw-   0        0        0     3080 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.8/test/test_filter_attributes.py
--rw-rw-rw-   0        0        0     1257 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.8/test/test_manager.py
--rw-rw-rw-   0        0        0      614 2024-01-05 23:56:06.000000 vectara-skunk-client-0.4.8/test/test_none_bool.py
--rw-rw-rw-   0        0        0     9025 2024-01-12 21:20:03.000000 vectara-skunk-client-0.4.8/test/test_query.py
--rw-rw-rw-   0        0        0      313 2023-12-29 23:40:50.000000 vectara-skunk-client-0.4.8/test/test_scratch.py
--rw-rw-rw-   0        0        0     2476 2024-01-04 21:17:59.000000 vectara-skunk-client-0.4.8/test/test_storage_quota.py
--rw-rw-rw-   0        0        0     2406 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.8/test/test_system_basic.py
--rw-rw-rw-   0        0        0     4780 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.8/test/test_util.py
-drwxrwxrwx   0        0        0        0 2024-01-12 21:27:24.447493 vectara-skunk-client-0.4.8/vectara/
--rw-rw-rw-   0        0        0        0 2023-12-22 03:08:32.000000 vectara-skunk-client-0.4.8/vectara/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 21:27:24.466405 vectara-skunk-client-0.4.8/vectara_skunk_client.egg-info/
--rw-rw-rw-   0        0        0      911 2024-01-12 21:27:24.000000 vectara-skunk-client-0.4.8/vectara_skunk_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      544 2024-01-12 21:27:24.000000 vectara-skunk-client-0.4.8/vectara_skunk_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-12 21:27:24.000000 vectara-skunk-client-0.4.8/vectara_skunk_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2024-01-12 21:27:24.000000 vectara-skunk-client-0.4.8/vectara_skunk_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-01-12 21:27:24.000000 vectara-skunk-client-0.4.8/vectara_skunk_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-01-12 21:39:23.366252 vectara-skunk-client-0.4.9/
+-rw-rw-rw-   0        0        0    34918 2023-12-21 21:26:20.000000 vectara-skunk-client-0.4.9/LICENSE.md
+-rw-rw-rw-   0        0        0      911 2024-01-12 21:39:23.365186 vectara-skunk-client-0.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5222 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-01-12 21:39:23.366252 vectara-skunk-client-0.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1379 2024-01-12 21:38:33.000000 vectara-skunk-client-0.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-12 21:39:23.330890 vectara-skunk-client-0.4.9/test/
+-rw-rw-rw-   0        0        0     5280 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/test/test_api_keys.py
+-rw-rw-rw-   0        0        0     2400 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/test/test_arabic.py
+-rw-rw-rw-   0        0        0     1348 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/test/test_basic_query.py
+-rw-rw-rw-   0        0        0     1395 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/test/test_documents.py
+-rw-rw-rw-   0        0        0     3080 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/test/test_filter_attributes.py
+-rw-rw-rw-   0        0        0     1257 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/test/test_manager.py
+-rw-rw-rw-   0        0        0      614 2024-01-05 23:56:06.000000 vectara-skunk-client-0.4.9/test/test_none_bool.py
+-rw-rw-rw-   0        0        0     9025 2024-01-12 21:20:03.000000 vectara-skunk-client-0.4.9/test/test_query.py
+-rw-rw-rw-   0        0        0      313 2023-12-29 23:40:50.000000 vectara-skunk-client-0.4.9/test/test_scratch.py
+-rw-rw-rw-   0        0        0     2476 2024-01-04 21:17:59.000000 vectara-skunk-client-0.4.9/test/test_storage_quota.py
+-rw-rw-rw-   0        0        0     2406 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/test/test_system_basic.py
+-rw-rw-rw-   0        0        0     4780 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/test/test_util.py
+drwxrwxrwx   0        0        0        0 2024-01-12 21:39:23.331951 vectara-skunk-client-0.4.9/vectara/
+-rw-rw-rw-   0        0        0        0 2023-12-22 03:08:32.000000 vectara-skunk-client-0.4.9/vectara/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-12 21:39:23.345756 vectara-skunk-client-0.4.9/vectara/client/
+-rw-rw-rw-   0        0        0        0 2024-01-12 21:18:54.000000 vectara-skunk-client-0.4.9/vectara/client/__init__.py
+-rw-rw-rw-   0        0        0     7940 2024-01-12 21:20:43.000000 vectara-skunk-client-0.4.9/vectara/client/admin.py
+-rw-rw-rw-   0        0        0     4266 2023-12-28 02:17:55.000000 vectara-skunk-client-0.4.9/vectara/client/authn.py
+-rw-rw-rw-   0        0        0     2157 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/vectara/client/chat.py
+-rw-rw-rw-   0        0        0     7525 2023-12-29 00:18:13.000000 vectara-skunk-client-0.4.9/vectara/client/config.py
+-rw-rw-rw-   0        0        0     4337 2024-01-12 21:20:03.000000 vectara-skunk-client-0.4.9/vectara/client/core.py
+-rw-rw-rw-   0        0        0     3173 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/vectara/client/dao.py
+-rw-rw-rw-   0        0        0     1472 2024-01-12 21:21:41.000000 vectara-skunk-client-0.4.9/vectara/client/document.py
+-rw-rw-rw-   0        0        0    10583 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/vectara/client/domain.py
+-rw-rw-rw-   0        0        0      640 2024-01-05 05:12:20.000000 vectara-skunk-client-0.4.9/vectara/client/enums.py
+-rw-rw-rw-   0        0        0        0 2024-01-04 05:06:30.000000 vectara-skunk-client-0.4.9/vectara/client/error.py
+-rw-rw-rw-   0        0        0     3886 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/vectara/client/index.py
+-rw-rw-rw-   0        0        0     1593 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/vectara/client/manager.py
+-rw-rw-rw-   0        0        0     5301 2024-01-12 21:21:14.000000 vectara-skunk-client-0.4.9/vectara/client/query.py
+-rw-rw-rw-   0        0        0     5131 2024-01-12 05:54:06.000000 vectara-skunk-client-0.4.9/vectara/client/status.py
+-rw-rw-rw-   0        0        0    19359 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/vectara/client/util.py
+drwxrwxrwx   0        0        0        0 2024-01-12 21:39:23.364120 vectara-skunk-client-0.4.9/vectara_skunk_client.egg-info/
+-rw-rw-rw-   0        0        0      911 2024-01-12 21:39:23.000000 vectara-skunk-client-0.4.9/vectara_skunk_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2024-01-12 21:39:23.000000 vectara-skunk-client-0.4.9/vectara_skunk_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-12 21:39:23.000000 vectara-skunk-client-0.4.9/vectara_skunk_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2024-01-12 21:39:23.000000 vectara-skunk-client-0.4.9/vectara_skunk_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-01-12 21:39:23.000000 vectara-skunk-client-0.4.9/vectara_skunk_client.egg-info/top_level.txt
```

### Comparing `vectara-skunk-client-0.4.8/LICENSE.md` & `vectara-skunk-client-0.4.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vectara-skunk-client-0.4.8/PKG-INFO` & `vectara-skunk-client-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara-skunk-client
-Version: 0.4.8
+Version: 0.4.9
 Summary: Vectara Skunk Client
 Home-page: https://github.com/davidglevy/vectara-skunk-client
 Author: David Levy
 Author-email: david.g.levy@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE v3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `vectara-skunk-client-0.4.8/README.md` & `vectara-skunk-client-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `vectara-skunk-client-0.4.8/setup.py` & `vectara-skunk-client-0.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,21 @@
         return "\n".join(lines)
 
 setup(
     name='vectara-skunk-client',
     description='Vectara Skunk Client',
     long_description=get_long_desc(),
     long_description_content_type='text/markdown',
-    version='0.4.8',
+    version='0.4.9',
     author='David Levy',
     author_email='david.g.levy@gmail.com',
     url='https://github.com/davidglevy/vectara-skunk-client',
     license='GNU AFFERO GENERAL PUBLIC LICENSE v3',
     package_dir={
-        'vectara.client': 'vectara'
+        'vectara.client': 'vectara/client'
     },
     packages=['vectara.client'],
     install_requires=['requests', 'dacite>=1.8.1', 'Authlib==1.0.1', 'pyaml==23.9.7', 'tqdm==4.66.1',
                       'requests-toolbelt==1.0.0'],
     python_requires='>=3.4',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
```

### Comparing `vectara-skunk-client-0.4.8/test/test_api_keys.py` & `vectara-skunk-client-0.4.9/test/test_api_keys.py`

 * *Files identical despite different names*

### Comparing `vectara-skunk-client-0.4.8/test/test_arabic.py` & `vectara-skunk-client-0.4.9/test/test_arabic.py`

 * *Files identical despite different names*

### Comparing `vectara-skunk-client-0.4.8/test/test_basic_query.py` & `vectara-skunk-client-0.4.9/test/test_basic_query.py`

 * *Files identical despite different names*

### Comparing `vectara-skunk-client-0.4.8/test/test_documents.py` & `vectara-skunk-client-0.4.9/test/test_documents.py`

 * *Files identical despite different names*

### Comparing `vectara-skunk-client-0.4.8/test/test_filter_attributes.py` & `vectara-skunk-client-0.4.9/test/test_filter_attributes.py`

 * *Files identical despite different names*

### Comparing `vectara-skunk-client-0.4.8/test/test_manager.py` & `vectara-skunk-client-0.4.9/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `vectara-skunk-client-0.4.8/test/test_none_bool.py` & `vectara-skunk-client-0.4.9/test/test_none_bool.py`

 * *Files identical despite different names*

### Comparing `vectara-skunk-client-0.4.8/test/test_query.py` & `vectara-skunk-client-0.4.9/test/test_query.py`

 * *Files identical despite different names*

### Comparing `vectara-skunk-client-0.4.8/test/test_storage_quota.py` & `vectara-skunk-client-0.4.9/test/test_storage_quota.py`

 * *Files identical despite different names*

### Comparing `vectara-skunk-client-0.4.8/test/test_system_basic.py` & `vectara-skunk-client-0.4.9/test/test_system_basic.py`

 * *Files identical despite different names*

### Comparing `vectara-skunk-client-0.4.8/test/test_util.py` & `vectara-skunk-client-0.4.9/test/test_util.py`

 * *Files identical despite different names*

### Comparing `vectara-skunk-client-0.4.8/vectara_skunk_client.egg-info/PKG-INFO` & `vectara-skunk-client-0.4.9/vectara_skunk_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara-skunk-client
-Version: 0.4.8
+Version: 0.4.9
 Summary: Vectara Skunk Client
 Home-page: https://github.com/davidglevy/vectara-skunk-client
 Author: David Levy
 Author-email: david.g.levy@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE v3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

