# Comparing `tmp/gen_wrappers-0.1.1.tar.gz` & `tmp/gen_wrappers-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.1.1.tar", last modified: Thu May  2 18:20:00 2024, max compression
+gzip compressed data, was "gen_wrappers-0.1.2.tar", last modified: Thu May  2 19:33:44 2024, max compression
```

## Comparing `gen_wrappers-0.1.1.tar` & `gen_wrappers-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 18:20:00.355773 gen_wrappers-0.1.1/
--rw-rw-rw-   0        0        0      823 2024-05-02 18:20:00.352771 gen_wrappers-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 18:20:00.226155 gen_wrappers-0.1.1/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.1.1/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 18:20:00.244409 gen_wrappers-0.1.1/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.1.1/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     5719 2024-05-02 16:04:46.000000 gen_wrappers-0.1.1/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     2193 2024-05-02 18:19:46.000000 gen_wrappers-0.1.1/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.1.1/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-02 18:20:00.265525 gen_wrappers-0.1.1/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.1.1/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1253 2024-05-02 15:57:38.000000 gen_wrappers-0.1.1/creator/base/base_app.py
--rw-rw-rw-   0        0        0      107 2024-05-02 17:56:22.000000 gen_wrappers-0.1.1/creator/base/base_request.py
--rw-rw-rw-   0        0        0     1569 2024-05-02 16:04:46.000000 gen_wrappers-0.1.1/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.1.1/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-02 18:20:00.286063 gen_wrappers-0.1.1/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.1.1/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9969 2024-05-02 16:04:46.000000 gen_wrappers-0.1.1/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0     2796 2024-05-02 18:19:46.000000 gen_wrappers-0.1.1/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.1.1/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-02 18:20:00.307841 gen_wrappers-0.1.1/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.1.1/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6340 2024-05-02 16:04:46.000000 gen_wrappers-0.1.1/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3968 2024-05-02 18:19:46.000000 gen_wrappers-0.1.1/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.1.1/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-02 18:20:00.348135 gen_wrappers-0.1.1/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      823 2024-05-02 18:20:00.000000 gen_wrappers-0.1.1/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2024-05-02 18:20:00.000000 gen_wrappers-0.1.1/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 18:20:00.000000 gen_wrappers-0.1.1/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-02 18:20:00.000000 gen_wrappers-0.1.1/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-02 18:20:00.000000 gen_wrappers-0.1.1/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 18:20:00.355773 gen_wrappers-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1015 2024-05-02 18:19:46.000000 gen_wrappers-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:33:44.980834 gen_wrappers-0.1.2/
+-rw-rw-rw-   0        0        0      823 2024-05-02 19:33:44.977627 gen_wrappers-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 19:33:44.862383 gen_wrappers-0.1.2/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.1.2/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:33:44.875268 gen_wrappers-0.1.2/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.1.2/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     5719 2024-05-02 16:04:46.000000 gen_wrappers-0.1.2/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     2193 2024-05-02 18:19:46.000000 gen_wrappers-0.1.2/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.1.2/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:33:44.888704 gen_wrappers-0.1.2/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.1.2/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1253 2024-05-02 15:57:38.000000 gen_wrappers-0.1.2/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      508 2024-05-02 19:33:29.000000 gen_wrappers-0.1.2/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     1569 2024-05-02 16:04:46.000000 gen_wrappers-0.1.2/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.1.2/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:33:44.898512 gen_wrappers-0.1.2/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.1.2/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9969 2024-05-02 16:04:46.000000 gen_wrappers-0.1.2/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0     2796 2024-05-02 18:19:46.000000 gen_wrappers-0.1.2/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.1.2/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:33:44.909563 gen_wrappers-0.1.2/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.1.2/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6340 2024-05-02 16:04:46.000000 gen_wrappers-0.1.2/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3968 2024-05-02 18:19:46.000000 gen_wrappers-0.1.2/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.1.2/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:33:44.972357 gen_wrappers-0.1.2/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      823 2024-05-02 19:33:44.000000 gen_wrappers-0.1.2/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      710 2024-05-02 19:33:44.000000 gen_wrappers-0.1.2/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 19:33:44.000000 gen_wrappers-0.1.2/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-02 19:33:44.000000 gen_wrappers-0.1.2/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-02 19:33:44.000000 gen_wrappers-0.1.2/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 19:33:44.980834 gen_wrappers-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2024-05-02 19:33:29.000000 gen_wrappers-0.1.2/setup.py
```

### Comparing `gen_wrappers-0.1.1/PKG-INFO` & `gen_wrappers-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.1.1
+Version: 0.1.2
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.1.1/creator/auto/creator_auto.py` & `gen_wrappers-0.1.2/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.1/creator/auto/request_auto.py` & `gen_wrappers-0.1.2/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.1/creator/auto/response_auto.py` & `gen_wrappers-0.1.2/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.1/creator/base/base_app.py` & `gen_wrappers-0.1.2/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.1/creator/base/base_response.py` & `gen_wrappers-0.1.2/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.1/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.1.2/creator/cmfy/creator_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.1/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.1.2/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.1/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.1.2/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.1/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.1.2/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.1/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.1.2/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.1/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.1.2/gen_wrappers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.1.1
+Version: 0.1.2
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.1.1/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.1.2/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.1/setup.py` & `gen_wrappers-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.1.1',
+    version='0.1.2',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```

