# Comparing `tmp/templated_setup-0.961.tar.gz` & `tmp/templated_setup-0.962.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.961.tar", last modified: Thu May  2 09:43:36 2024, max compression
+gzip compressed data, was "templated_setup-0.962.tar", last modified: Thu May  2 09:46:44 2024, max compression
```

## Comparing `templated_setup-0.961.tar` & `templated_setup-0.962.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:43:36.285005 templated_setup-0.961/
--rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.961/LICENCE
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:43:36.283887 templated_setup-0.961/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.961/README.md
--rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 09:43:36.285161 templated_setup-0.961/setup.cfg
--rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.961/setup.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:43:36.239311 templated_setup-0.961/templated_setup/
--rw-r--r--   0 joel-watson   (501) staff       (20)    17269 2024-05-02 09:43:01.000000 templated_setup-0.961/templated_setup/__init__.py
--rw-r--r--   0 joel-watson   (501) staff       (20)       21 2024-05-02 09:43:34.000000 templated_setup-0.961/templated_setup/_hardcoded_version.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:43:36.282462 templated_setup-0.961/templated_setup.egg-info/
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:43:35.000000 templated_setup-0.961/templated_setup.egg-info/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)      248 2024-05-02 09:43:35.000000 templated_setup-0.961/templated_setup.egg-info/SOURCES.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 09:43:35.000000 templated_setup-0.961/templated_setup.egg-info/dependency_links.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 09:43:35.000000 templated_setup-0.961/templated_setup.egg-info/top_level.txt
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:46:44.157474 templated_setup-0.962/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.962/LICENCE
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:46:44.156451 templated_setup-0.962/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.962/README.md
+-rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 09:46:44.157646 templated_setup-0.962/setup.cfg
+-rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.962/setup.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:46:44.153161 templated_setup-0.962/templated_setup/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    17267 2024-05-02 09:45:41.000000 templated_setup-0.962/templated_setup/__init__.py
+-rw-r--r--   0 joel-watson   (501) staff       (20)       21 2024-05-02 09:46:43.000000 templated_setup-0.962/templated_setup/_hardcoded_version.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:46:44.155791 templated_setup-0.962/templated_setup.egg-info/
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:46:44.000000 templated_setup-0.962/templated_setup.egg-info/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)      248 2024-05-02 09:46:44.000000 templated_setup-0.962/templated_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 09:46:44.000000 templated_setup-0.962/templated_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 09:46:44.000000 templated_setup-0.962/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.961/LICENCE` & `templated_setup-0.962/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.961/PKG-INFO` & `templated_setup-0.962/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.961
+Version: 0.962
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
 
-## V0.961 released on 2nd/5/2024
+## V0.962 released on 2nd/5/2024
 god please kill me. ;(
```

### Comparing `templated_setup-0.961/README.md` & `templated_setup-0.962/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.961/templated_setup/__init__.py` & `templated_setup-0.962/templated_setup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -636,16 +636,16 @@
 	def _handle_installation_via_pip(cls, name):
 
 		# NOTE: If we do not hardcode the version, then pip will throw a fit when trying to install the 
 		# NOTE:   `templated-setup` package.
 		from . import _hardcoded_version
 
 		setup(
-			name=_hardcoded_version.__version__, #type:ignore
-			version="0.960"
+			name=name,
+			version=_hardcoded_version.__version__, #type:ignore
 		)
 
 		return None
 	
 		f"[ END ] {_Setup_Helper._handle_installation_via_pip}"
```

### Comparing `templated_setup-0.961/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.962/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.961
+Version: 0.962
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
 
-## V0.961 released on 2nd/5/2024
+## V0.962 released on 2nd/5/2024
 god please kill me. ;(
```

