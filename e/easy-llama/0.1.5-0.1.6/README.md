# Comparing `tmp/easy_llama-0.1.5.tar.gz` & `tmp/easy_llama-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_llama-0.1.5.tar", last modified: Wed May  1 06:59:37 2024, max compression
+gzip compressed data, was "easy_llama-0.1.6.tar", last modified: Thu May  2 15:12:04 2024, max compression
```

## Comparing `easy_llama-0.1.5.tar` & `easy_llama-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-01 06:59:37.203362 easy_llama-0.1.5/
--rw-r--r--   0 dylan      (501) staff       (20)     1211 2024-04-30 22:20:53.000000 easy_llama-0.1.5/LICENSE
--rw-r--r--   0 dylan      (501) staff       (20)     1085 2024-05-01 06:59:37.203133 easy_llama-0.1.5/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)    13483 2024-05-01 06:55:26.000000 easy_llama-0.1.5/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-01 06:59:37.202092 easy_llama-0.1.5/easy_llama/
--rw-r--r--   0 dylan      (501) staff       (20)      241 2024-05-01 06:50:15.000000 easy_llama-0.1.5/easy_llama/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)    16378 2024-04-30 21:53:31.000000 easy_llama-0.1.5/easy_llama/formats.py
--rw-r--r--   0 dylan      (501) staff       (20)    24212 2024-04-30 21:53:32.000000 easy_llama-0.1.5/easy_llama/model.py
--rw-r--r--   0 dylan      (501) staff       (20)     4053 2024-04-30 21:53:34.000000 easy_llama-0.1.5/easy_llama/samplers.py
--rw-r--r--   0 dylan      (501) staff       (20)    21726 2024-05-01 06:46:41.000000 easy_llama-0.1.5/easy_llama/thread.py
--rw-r--r--   0 dylan      (501) staff       (20)     4731 2024-04-30 21:53:43.000000 easy_llama-0.1.5/easy_llama/utils.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-01 06:59:37.202865 easy_llama-0.1.5/easy_llama.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)     1085 2024-05-01 06:59:37.000000 easy_llama-0.1.5/easy_llama.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      324 2024-05-01 06:59:37.000000 easy_llama-0.1.5/easy_llama.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2024-05-01 06:59:37.000000 easy_llama-0.1.5/easy_llama.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)       26 2024-05-01 06:59:37.000000 easy_llama-0.1.5/easy_llama.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)       11 2024-05-01 06:59:37.000000 easy_llama-0.1.5/easy_llama.egg-info/top_level.txt
--rw-r--r--   0 dylan      (501) staff       (20)       38 2024-05-01 06:59:37.203405 easy_llama-0.1.5/setup.cfg
--rw-r--r--   0 dylan      (501) staff       (20)     1212 2024-05-01 06:50:34.000000 easy_llama-0.1.5/setup.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-02 15:12:04.949412 easy_llama-0.1.6/
+-rw-r--r--   0 dylan      (501) staff       (20)     1211 2024-04-30 22:20:53.000000 easy_llama-0.1.6/LICENSE
+-rw-r--r--   0 dylan      (501) staff       (20)     1085 2024-05-02 15:12:04.949192 easy_llama-0.1.6/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)    13482 2024-05-01 08:34:07.000000 easy_llama-0.1.6/README.md
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-02 15:12:04.948145 easy_llama-0.1.6/easy_llama/
+-rw-r--r--   0 dylan      (501) staff       (20)      241 2024-05-02 15:11:16.000000 easy_llama-0.1.6/easy_llama/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)    16378 2024-04-30 21:53:31.000000 easy_llama-0.1.6/easy_llama/formats.py
+-rw-r--r--   0 dylan      (501) staff       (20)    24212 2024-04-30 21:53:32.000000 easy_llama-0.1.6/easy_llama/model.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4053 2024-04-30 21:53:34.000000 easy_llama-0.1.6/easy_llama/samplers.py
+-rw-r--r--   0 dylan      (501) staff       (20)    21726 2024-05-01 06:46:41.000000 easy_llama-0.1.6/easy_llama/thread.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4731 2024-04-30 21:53:43.000000 easy_llama-0.1.6/easy_llama/utils.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-02 15:12:04.948995 easy_llama-0.1.6/easy_llama.egg-info/
+-rw-r--r--   0 dylan      (501) staff       (20)     1085 2024-05-02 15:12:04.000000 easy_llama-0.1.6/easy_llama.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      324 2024-05-02 15:12:04.000000 easy_llama-0.1.6/easy_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2024-05-02 15:12:04.000000 easy_llama-0.1.6/easy_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       26 2024-05-02 15:12:04.000000 easy_llama-0.1.6/easy_llama.egg-info/requires.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       11 2024-05-02 15:12:04.000000 easy_llama-0.1.6/easy_llama.egg-info/top_level.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       38 2024-05-02 15:12:04.949460 easy_llama-0.1.6/setup.cfg
+-rw-r--r--   0 dylan      (501) staff       (20)     1212 2024-05-02 15:11:19.000000 easy_llama-0.1.6/setup.py
```

### Comparing `easy_llama-0.1.5/LICENSE` & `easy_llama-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_llama-0.1.5/PKG-INFO` & `easy_llama-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_llama
-Version: 0.1.5
+Version: 0.1.6
 Summary: Text generation in Python, made easy
 Home-page: https://github.com/ddh0/easy-llama/
 Author: Dylan Halladay
 Author-email: dylanhalladay02@icloud.com
 License: The Unlicense
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `easy_llama-0.1.5/README.md` & `easy_llama-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
   > 
 ```
 
 ## Installing with pip
 
 In most cases, the best way to install easy-llama is through pip.
 
-Select your backend from the list below to see your installation instructions. If you run into issues with the installation, please see the [llama-cpp-python installation instructions](https://github.com/abetlen/llama-cpp-python?tab=readme-ov-file#installation)  for a more detailed guide. If you're still having trouble, feel free to [open an issue](https://github.com/ddh0/easy-llama/issues/new/).
+Select your backend from the list below to see your installation instructions. If you run into issues with the installation, please see the [llama-cpp-python installation instructions](https://github.com/abetlen/llama-cpp-python?tab=readme-ov-file#installation) for a more detailed guide. If you're still having trouble, feel free to [open an issue](https://github.com/ddh0/easy-llama/issues/new/).
 
 <details>
 <summary>CPU only</summary>
 
 ```
 pip install easy-llama
 ```
```

### Comparing `easy_llama-0.1.5/easy_llama/formats.py` & `easy_llama-0.1.6/easy_llama/formats.py`

 * *Files identical despite different names*

### Comparing `easy_llama-0.1.5/easy_llama/model.py` & `easy_llama-0.1.6/easy_llama/model.py`

 * *Files identical despite different names*

### Comparing `easy_llama-0.1.5/easy_llama/samplers.py` & `easy_llama-0.1.6/easy_llama/samplers.py`

 * *Files identical despite different names*

### Comparing `easy_llama-0.1.5/easy_llama/thread.py` & `easy_llama-0.1.6/easy_llama/thread.py`

 * *Files identical despite different names*

### Comparing `easy_llama-0.1.5/easy_llama/utils.py` & `easy_llama-0.1.6/easy_llama/utils.py`

 * *Files identical despite different names*

### Comparing `easy_llama-0.1.5/easy_llama.egg-info/PKG-INFO` & `easy_llama-0.1.6/easy_llama.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_llama
-Version: 0.1.5
+Version: 0.1.6
 Summary: Text generation in Python, made easy
 Home-page: https://github.com/ddh0/easy-llama/
 Author: Dylan Halladay
 Author-email: dylanhalladay02@icloud.com
 License: The Unlicense
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `easy_llama-0.1.5/setup.py` & `easy_llama-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='easy_llama',
-    version='0.1.5',
+    version='0.1.6',
     description='Text generation in Python, made easy',
     long_description="""To view the current documentation for easy-llama, visit the project's GitHub repository:\nhttps://github.com/ddh0/easy-llama""",
     url='https://github.com/ddh0/easy-llama/',
     author='Dylan Halladay',
     author_email='dylanhalladay02@icloud.com',
     license='The Unlicense',
     packages=['easy_llama'],
```

