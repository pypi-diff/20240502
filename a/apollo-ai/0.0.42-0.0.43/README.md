# Comparing `tmp/apollo-ai-0.0.42.tar.gz` & `tmp/apollo-ai-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-ai-0.0.42.tar", last modified: Thu May  2 15:20:24 2024, max compression
+gzip compressed data, was "apollo-ai-0.0.43.tar", last modified: Thu May  2 15:33:49 2024, max compression
```

## Comparing `apollo-ai-0.0.42.tar` & `apollo-ai-0.0.43.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 15:20:24.176377 apollo-ai-0.0.42/
--rw-rw-rw-   0        0        0    35823 2023-09-19 22:57:32.000000 apollo-ai-0.0.42/LICENSE
--rw-rw-rw-   0        0        0     9511 2024-05-02 15:20:24.173363 apollo-ai-0.0.42/PKG-INFO
--rw-rw-rw-   0        0        0     8994 2023-11-08 20:42:11.000000 apollo-ai-0.0.42/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 15:20:24.114786 apollo-ai-0.0.42/apollo/
-drwxrwxrwx   0        0        0        0 2024-05-02 15:20:24.138384 apollo-ai-0.0.42/apollo/apollo_ai.egg-info/
--rw-rw-rw-   0        0        0     9511 2024-05-02 15:20:23.000000 apollo-ai-0.0.42/apollo/apollo_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2024-05-02 15:20:23.000000 apollo-ai-0.0.42/apollo/apollo_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 15:20:23.000000 apollo-ai-0.0.42/apollo/apollo_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      596 2024-05-02 15:20:23.000000 apollo-ai-0.0.42/apollo/apollo_ai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-02 15:20:23.000000 apollo-ai-0.0.42/apollo/apollo_ai.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 15:20:24.149367 apollo-ai-0.0.42/apollo/argus/
--rw-rw-rw-   0        0        0       65 2024-05-02 14:32:40.000000 apollo-ai-0.0.42/apollo/argus/__init__.py
--rw-rw-rw-   0        0        0    12224 2024-05-02 14:32:40.000000 apollo-ai-0.0.42/apollo/argus/argus.py
--rw-rw-rw-   0        0        0     6904 2024-05-02 14:32:40.000000 apollo-ai-0.0.42/apollo/argus/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:20:24.159363 apollo-ai-0.0.42/apollo/lyre/
--rw-rw-rw-   0        0        0      233 2023-11-11 21:10:51.000000 apollo-ai-0.0.42/apollo/lyre/__init__.py
--rw-rw-rw-   0        0        0    13458 2024-05-02 14:32:40.000000 apollo-ai-0.0.42/apollo/lyre/lyre.py
--rw-rw-rw-   0        0        0      848 2023-11-10 23:08:26.000000 apollo-ai-0.0.42/apollo/lyre/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:20:24.169365 apollo-ai-0.0.42/apollo/pythia/
--rw-rw-rw-   0        0        0      201 2024-05-02 14:32:40.000000 apollo-ai-0.0.42/apollo/pythia/__init__.py
--rw-rw-rw-   0        0        0    10013 2024-05-02 14:32:40.000000 apollo-ai-0.0.42/apollo/pythia/pythia.py
--rw-rw-rw-   0        0        0     4339 2024-05-02 14:32:40.000000 apollo-ai-0.0.42/apollo/pythia/utils.py
--rw-rw-rw-   0        0        0       42 2024-05-02 15:20:24.176377 apollo-ai-0.0.42/setup.cfg
--rw-rw-rw-   0        0        0     1004 2024-05-02 15:20:20.000000 apollo-ai-0.0.42/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:33:49.318270 apollo-ai-0.0.43/
+-rw-rw-rw-   0        0        0    35823 2023-09-19 22:57:32.000000 apollo-ai-0.0.43/LICENSE
+-rw-rw-rw-   0        0        0     9511 2024-05-02 15:33:49.317214 apollo-ai-0.0.43/PKG-INFO
+-rw-rw-rw-   0        0        0     8994 2023-11-08 20:42:11.000000 apollo-ai-0.0.43/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 15:33:49.261862 apollo-ai-0.0.43/apollo/
+drwxrwxrwx   0        0        0        0 2024-05-02 15:33:49.285192 apollo-ai-0.0.43/apollo/apollo_ai.egg-info/
+-rw-rw-rw-   0        0        0     9511 2024-05-02 15:33:48.000000 apollo-ai-0.0.43/apollo/apollo_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2024-05-02 15:33:49.000000 apollo-ai-0.0.43/apollo/apollo_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 15:33:48.000000 apollo-ai-0.0.43/apollo/apollo_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      596 2024-05-02 15:33:48.000000 apollo-ai-0.0.43/apollo/apollo_ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-02 15:33:48.000000 apollo-ai-0.0.43/apollo/apollo_ai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 15:33:49.295202 apollo-ai-0.0.43/apollo/argus/
+-rw-rw-rw-   0        0        0       65 2024-05-02 14:32:40.000000 apollo-ai-0.0.43/apollo/argus/__init__.py
+-rw-rw-rw-   0        0        0    12224 2024-05-02 14:32:40.000000 apollo-ai-0.0.43/apollo/argus/argus.py
+-rw-rw-rw-   0        0        0     6904 2024-05-02 14:32:40.000000 apollo-ai-0.0.43/apollo/argus/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:33:49.305206 apollo-ai-0.0.43/apollo/lyre/
+-rw-rw-rw-   0        0        0      233 2023-11-11 21:10:51.000000 apollo-ai-0.0.43/apollo/lyre/__init__.py
+-rw-rw-rw-   0        0        0    13458 2024-05-02 14:32:40.000000 apollo-ai-0.0.43/apollo/lyre/lyre.py
+-rw-rw-rw-   0        0        0      848 2023-11-10 23:08:26.000000 apollo-ai-0.0.43/apollo/lyre/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:33:49.313173 apollo-ai-0.0.43/apollo/pythia/
+-rw-rw-rw-   0        0        0      201 2024-05-02 14:32:40.000000 apollo-ai-0.0.43/apollo/pythia/__init__.py
+-rw-rw-rw-   0        0        0    10013 2024-05-02 14:32:40.000000 apollo-ai-0.0.43/apollo/pythia/pythia.py
+-rw-rw-rw-   0        0        0     4339 2024-05-02 14:32:40.000000 apollo-ai-0.0.43/apollo/pythia/utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-02 15:33:49.318270 apollo-ai-0.0.43/setup.cfg
+-rw-rw-rw-   0        0        0      977 2024-05-02 15:33:37.000000 apollo-ai-0.0.43/setup.py
```

### Comparing `apollo-ai-0.0.42/LICENSE` & `apollo-ai-0.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.42/PKG-INFO` & `apollo-ai-0.0.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-ai
-Version: 0.0.42
+Version: 0.0.43
 Summary: Framework to process 3 channels in one: Video, Audio & Text
 Home-page: https://github.com/VerbaNexAI/APOLLO.AI
 Author: VerbaNex, Riddle
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-ai-0.0.42/README.md` & `apollo-ai-0.0.43/README.md`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.42/apollo/apollo_ai.egg-info/PKG-INFO` & `apollo-ai-0.0.43/apollo/apollo_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-ai
-Version: 0.0.42
+Version: 0.0.43
 Summary: Framework to process 3 channels in one: Video, Audio & Text
 Home-page: https://github.com/VerbaNexAI/APOLLO.AI
 Author: VerbaNex, Riddle
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-ai-0.0.42/apollo/apollo_ai.egg-info/requires.txt` & `apollo-ai-0.0.43/apollo/apollo_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.42/apollo/argus/argus.py` & `apollo-ai-0.0.43/apollo/argus/argus.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.42/apollo/argus/utils.py` & `apollo-ai-0.0.43/apollo/argus/utils.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.42/apollo/lyre/lyre.py` & `apollo-ai-0.0.43/apollo/lyre/lyre.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.42/apollo/lyre/utils.py` & `apollo-ai-0.0.43/apollo/lyre/utils.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.42/apollo/pythia/pythia.py` & `apollo-ai-0.0.43/apollo/pythia/pythia.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.42/apollo/pythia/utils.py` & `apollo-ai-0.0.43/apollo/pythia/utils.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.42/setup.py` & `apollo-ai-0.0.43/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 with open("requirements.txt", "r", encoding='utf-16') as f:
     required = f.read().splitlines()
 
-print(long_description)
-
 setup(
     name="apollo-ai",
-    version="0.0.42",
+    version="0.0.43",
     description="Framework to process 3 channels in one: Video, Audio & Text",
     package_dir={"": "apollo"},
     packages=find_packages(where="apollo"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/VerbaNexAI/APOLLO.AI",
     author="VerbaNex, Riddle",
```

