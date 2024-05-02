# Comparing `tmp/antidupe-0.0.6.tar.gz` & `tmp/antidupe-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antidupe-0.0.6.tar", last modified: Wed May  1 19:51:09 2024, max compression
+gzip compressed data, was "antidupe-0.0.7.tar", last modified: Wed May  1 20:11:30 2024, max compression
```

## Comparing `antidupe-0.0.6.tar` & `antidupe-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:09.219153 antidupe-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 19:50:58.000000 antidupe-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-01 19:51:09.219153 antidupe-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-01 19:50:58.000000 antidupe-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:09.219153 antidupe-0.0.6/antidupe/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 19:50:58.000000 antidupe-0.0.6/antidupe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-01 19:50:58.000000 antidupe-0.0.6/antidupe/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-01 19:50:58.000000 antidupe-0.0.6/antidupe/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:09.219153 antidupe-0.0.6/antidupe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-01 19:51:09.000000 antidupe-0.0.6/antidupe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-01 19:51:09.000000 antidupe-0.0.6/antidupe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:51:09.000000 antidupe-0.0.6/antidupe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-01 19:51:09.000000 antidupe-0.0.6/antidupe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 19:51:09.000000 antidupe-0.0.6/antidupe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:51:09.219153 antidupe-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-01 19:50:58.000000 antidupe-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:11:30.281825 antidupe-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 20:11:20.000000 antidupe-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-01 20:11:30.281825 antidupe-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-01 20:11:20.000000 antidupe-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:11:30.281825 antidupe-0.0.7/antidupe/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 20:11:20.000000 antidupe-0.0.7/antidupe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-01 20:11:20.000000 antidupe-0.0.7/antidupe/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-05-01 20:11:20.000000 antidupe-0.0.7/antidupe/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:11:30.281825 antidupe-0.0.7/antidupe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-01 20:11:30.000000 antidupe-0.0.7/antidupe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-01 20:11:30.000000 antidupe-0.0.7/antidupe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:11:30.000000 antidupe-0.0.7/antidupe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-01 20:11:30.000000 antidupe-0.0.7/antidupe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 20:11:30.000000 antidupe-0.0.7/antidupe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 20:11:30.281825 antidupe-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-01 20:11:20.000000 antidupe-0.0.7/setup.py
```

### Comparing `antidupe-0.0.6/LICENSE` & `antidupe-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `antidupe-0.0.6/PKG-INFO` & `antidupe-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antidupe
-Version: 0.0.6
+Version: 0.0.7
 Summary: Image deduplicator using CNN, Cosine Similarity, Image Hashing, Structural Similarity Index Measurement, and Euclidean Distance
 Home-page: https://github.com/manbehindthemadness/antidupe
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `antidupe-0.0.6/README.md` & `antidupe-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `antidupe-0.0.6/antidupe/main.py` & `antidupe-0.0.7/antidupe/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 DEFAULTS = {
     'ih': 0.1,
     'ssim': 0.15,
     'cs': 0.1,
     'cnn': 0.15,
-    'dedup': 0.85,
+    'dedup': 0.1,
 }
 
 
 class Antidupe:
     """
     Discover duplicate images.
     """
```

### Comparing `antidupe-0.0.6/antidupe/utilities.py` & `antidupe-0.0.7/antidupe/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,16 @@
         }
 
         similarity_score = self.cnn_encoder._find_duplicates_dict(  # noqa
             embeddings_dict,  # noqa
             min_similarity_threshold=threshold,
             scores=True
         )  # noqa
-        return similarity_score[1][0][1]
+        result = np.subtract(1.0, np.round(similarity_score[1][0][1], 4))
+        return result
 
 
 def test():
     """
     This will test the various math functions
     """
     cnn = CNN()
```

### Comparing `antidupe-0.0.6/antidupe.egg-info/PKG-INFO` & `antidupe-0.0.7/antidupe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antidupe
-Version: 0.0.6
+Version: 0.0.7
 Summary: Image deduplicator using CNN, Cosine Similarity, Image Hashing, Structural Similarity Index Measurement, and Euclidean Distance
 Home-page: https://github.com/manbehindthemadness/antidupe
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `antidupe-0.0.6/setup.py` & `antidupe-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='antidupe',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(),
     install_requires=install_requires,
     entry_points={
         'console_scripts': [
         ],
     },
     author='Manbehindthemadness',
```

