# Comparing `tmp/gen_wrappers-0.1.2.tar.gz` & `tmp/gen_wrappers-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.1.2.tar", last modified: Thu May  2 19:33:44 2024, max compression
+gzip compressed data, was "gen_wrappers-0.1.3.tar", last modified: Thu May  2 19:51:56 2024, max compression
```

## Comparing `gen_wrappers-0.1.2.tar` & `gen_wrappers-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 19:33:44.980834 gen_wrappers-0.1.2/
--rw-rw-rw-   0        0        0      823 2024-05-02 19:33:44.977627 gen_wrappers-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 19:33:44.862383 gen_wrappers-0.1.2/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.1.2/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 19:33:44.875268 gen_wrappers-0.1.2/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.1.2/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     5719 2024-05-02 16:04:46.000000 gen_wrappers-0.1.2/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     2193 2024-05-02 18:19:46.000000 gen_wrappers-0.1.2/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.1.2/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-02 19:33:44.888704 gen_wrappers-0.1.2/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.1.2/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1253 2024-05-02 15:57:38.000000 gen_wrappers-0.1.2/creator/base/base_app.py
--rw-rw-rw-   0        0        0      508 2024-05-02 19:33:29.000000 gen_wrappers-0.1.2/creator/base/base_request.py
--rw-rw-rw-   0        0        0     1569 2024-05-02 16:04:46.000000 gen_wrappers-0.1.2/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.1.2/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-02 19:33:44.898512 gen_wrappers-0.1.2/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.1.2/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9969 2024-05-02 16:04:46.000000 gen_wrappers-0.1.2/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0     2796 2024-05-02 18:19:46.000000 gen_wrappers-0.1.2/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.1.2/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-02 19:33:44.909563 gen_wrappers-0.1.2/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.1.2/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6340 2024-05-02 16:04:46.000000 gen_wrappers-0.1.2/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3968 2024-05-02 18:19:46.000000 gen_wrappers-0.1.2/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.1.2/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-02 19:33:44.972357 gen_wrappers-0.1.2/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      823 2024-05-02 19:33:44.000000 gen_wrappers-0.1.2/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2024-05-02 19:33:44.000000 gen_wrappers-0.1.2/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 19:33:44.000000 gen_wrappers-0.1.2/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-02 19:33:44.000000 gen_wrappers-0.1.2/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-02 19:33:44.000000 gen_wrappers-0.1.2/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 19:33:44.980834 gen_wrappers-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1015 2024-05-02 19:33:29.000000 gen_wrappers-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:51:56.776763 gen_wrappers-0.1.3/
+-rw-rw-rw-   0        0        0      823 2024-05-02 19:51:56.774769 gen_wrappers-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 19:51:56.681662 gen_wrappers-0.1.3/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.1.3/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:51:56.702481 gen_wrappers-0.1.3/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.1.3/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     5719 2024-05-02 16:04:46.000000 gen_wrappers-0.1.3/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     2193 2024-05-02 18:19:46.000000 gen_wrappers-0.1.3/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.1.3/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:51:56.716696 gen_wrappers-0.1.3/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.1.3/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1253 2024-05-02 15:57:38.000000 gen_wrappers-0.1.3/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.1.3/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     1569 2024-05-02 16:04:46.000000 gen_wrappers-0.1.3/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.1.3/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:51:56.726896 gen_wrappers-0.1.3/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.1.3/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9969 2024-05-02 16:04:46.000000 gen_wrappers-0.1.3/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0     2796 2024-05-02 18:19:46.000000 gen_wrappers-0.1.3/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.1.3/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:51:56.736416 gen_wrappers-0.1.3/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.1.3/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6340 2024-05-02 16:04:46.000000 gen_wrappers-0.1.3/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3970 2024-05-02 19:47:45.000000 gen_wrappers-0.1.3/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.1.3/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:51:56.770747 gen_wrappers-0.1.3/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      823 2024-05-02 19:51:56.000000 gen_wrappers-0.1.3/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      710 2024-05-02 19:51:56.000000 gen_wrappers-0.1.3/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 19:51:56.000000 gen_wrappers-0.1.3/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-02 19:51:56.000000 gen_wrappers-0.1.3/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-02 19:51:56.000000 gen_wrappers-0.1.3/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 19:51:56.776763 gen_wrappers-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2024-05-02 19:51:53.000000 gen_wrappers-0.1.3/setup.py
```

### Comparing `gen_wrappers-0.1.2/PKG-INFO` & `gen_wrappers-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.1.2
+Version: 0.1.3
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.1.2/creator/auto/creator_auto.py` & `gen_wrappers-0.1.3/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.2/creator/auto/request_auto.py` & `gen_wrappers-0.1.3/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.2/creator/auto/response_auto.py` & `gen_wrappers-0.1.3/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.2/creator/base/base_app.py` & `gen_wrappers-0.1.3/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.2/creator/base/base_response.py` & `gen_wrappers-0.1.3/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.2/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.1.3/creator/cmfy/creator_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.2/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.1.3/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.2/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.1.3/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.2/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.1.3/creator/fcus_api/request_fcus_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     app: str = "FCUS"
     request_params: str = ""
     input_image: str = ""
     input_mask: str = ""
     outpaint_selections: List[str] = Field(default_factory=list, examples=[])
     prompt: str = ""
     negative_prompt: str = ""
-    style_selections: List[str] = Field(default_factory=list, examples=["Fooocus V2", "Fooocus Enhance", "Fooocus Sharp"])
+    style_selections: List[str] = Field(default_factory=list, examples=[["Fooocus V2", "Fooocus Enhance", "Fooocus Sharp"]])
     performance_selection: str = ""
     aspect_ratios_selection: str = ""
     image_number: int = 1
     image_seed: int = -1
     sharpness: float = 0.0
     guidance_scale: float = 7.5
     base_model_name: str = "RunDiffusion-XL-Photo.safetensors"
```

### Comparing `gen_wrappers-0.1.2/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.1.3/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.2/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.1.3/gen_wrappers.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.1.2
+Version: 0.1.3
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.1.2/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.1.3/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.2/setup.py` & `gen_wrappers-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.1.2',
+    version='0.1.3',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```
