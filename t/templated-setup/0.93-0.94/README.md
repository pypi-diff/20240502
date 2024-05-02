# Comparing `tmp/templated_setup-0.93.tar.gz` & `tmp/templated_setup-0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.93.tar", last modified: Thu May  2 04:37:21 2024, max compression
+gzip compressed data, was "templated_setup-0.94.tar", last modified: Thu May  2 04:48:49 2024, max compression
```

## Comparing `templated_setup-0.93.tar` & `templated_setup-0.94.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 04:37:21.635780 templated_setup-0.93/
--rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.93/LICENCE
--rw-r--r--   0 joel-watson   (501) staff       (20)     2465 2024-05-02 04:37:21.635308 templated_setup-0.93/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.93/README.md
--rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 04:37:21.635869 templated_setup-0.93/setup.cfg
--rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:31:02.000000 templated_setup-0.93/setup.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 04:37:21.633247 templated_setup-0.93/templated_setup/
--rw-r--r--   0 joel-watson   (501) staff       (20)    19909 2024-05-02 04:36:57.000000 templated_setup-0.93/templated_setup/__init__.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 04:37:21.634927 templated_setup-0.93/templated_setup.egg-info/
--rw-r--r--   0 joel-watson   (501) staff       (20)     2465 2024-05-02 04:37:21.000000 templated_setup-0.93/templated_setup.egg-info/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)      210 2024-05-02 04:37:21.000000 templated_setup-0.93/templated_setup.egg-info/SOURCES.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 04:37:21.000000 templated_setup-0.93/templated_setup.egg-info/dependency_links.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 04:37:21.000000 templated_setup-0.93/templated_setup.egg-info/top_level.txt
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 04:48:49.311545 templated_setup-0.94/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.94/LICENCE
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2465 2024-05-02 04:48:49.310961 templated_setup-0.94/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.94/README.md
+-rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 04:48:49.311648 templated_setup-0.94/setup.cfg
+-rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:31:02.000000 templated_setup-0.94/setup.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 04:48:49.308488 templated_setup-0.94/templated_setup/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    19804 2024-05-02 04:48:43.000000 templated_setup-0.94/templated_setup/__init__.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 04:48:49.310494 templated_setup-0.94/templated_setup.egg-info/
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2465 2024-05-02 04:48:49.000000 templated_setup-0.94/templated_setup.egg-info/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)      210 2024-05-02 04:48:49.000000 templated_setup-0.94/templated_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 04:48:49.000000 templated_setup-0.94/templated_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 04:48:49.000000 templated_setup-0.94/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.93/LICENCE` & `templated_setup-0.94/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.93/PKG-INFO` & `templated_setup-0.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.93
+Version: 0.94
 Summary: A quick and easy replacement for some `setup.py` implementations.
 Author: matrikater (Joel Watson)
 Author-email: administraitor@matriko.xyz
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 
 # Standardized `setup.py`
@@ -65,9 +65,9 @@
 
 > Actually I would be happy to have some help with this project as making a `setup.py` every time is a bit boring.
 
 ## License
 
 This project is licensed under the GPLv2 License - see the [LICENSE](LICENSE) file for details.
 
-## V0.93 released on 2nd/5/2024
+## V0.94 released on 2nd/5/2024
 god please kill me. ;(
```

### Comparing `templated_setup-0.93/README.md` & `templated_setup-0.94/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.93/templated_setup/__init__.py` & `templated_setup-0.94/templated_setup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -591,17 +591,14 @@
 
 
 
 	@classmethod
 	def _load_from_hardcoded(cls):
 
 		cls._is_using_pip = False
-		if "VIRTUAL_ENV" in os.environ.keys():
-			if "pip" in ' '.join(sys.argv):
-				cls._is_using_pip = True
 		if "PIP_BUILD_TRACKER" in os.environ.keys():
 			cls._is_using_pip = True
 
 		try:
 			__ = cls._json_data
 		except AttributeError:
 			cls._json_data = None
```

### Comparing `templated_setup-0.93/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.94/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.93
+Version: 0.94
 Summary: A quick and easy replacement for some `setup.py` implementations.
 Author: matrikater (Joel Watson)
 Author-email: administraitor@matriko.xyz
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 
 # Standardized `setup.py`
@@ -65,9 +65,9 @@
 
 > Actually I would be happy to have some help with this project as making a `setup.py` every time is a bit boring.
 
 ## License
 
 This project is licensed under the GPLv2 License - see the [LICENSE](LICENSE) file for details.
 
-## V0.93 released on 2nd/5/2024
+## V0.94 released on 2nd/5/2024
 god please kill me. ;(
```

