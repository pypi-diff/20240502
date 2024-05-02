# Comparing `tmp/templated_setup-0.959.tar.gz` & `tmp/templated_setup-0.960.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.959.tar", last modified: Thu May  2 09:29:52 2024, max compression
+gzip compressed data, was "templated_setup-0.960.tar", last modified: Thu May  2 09:34:34 2024, max compression
```

## Comparing `templated_setup-0.959.tar` & `templated_setup-0.960.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:29:52.271745 templated_setup-0.959/
--rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.959/LICENCE
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:29:52.270955 templated_setup-0.959/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.959/README.md
--rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 09:29:52.271880 templated_setup-0.959/setup.cfg
--rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.959/setup.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:29:52.231965 templated_setup-0.959/templated_setup/
--rw-r--r--   0 joel-watson   (501) staff       (20)    16762 2024-05-02 09:29:11.000000 templated_setup-0.959/templated_setup/__init__.py
--rw-r--r--   0 joel-watson   (501) staff       (20)      144 2024-05-02 09:03:39.000000 templated_setup-0.959/templated_setup/_hardcoded.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:29:52.270498 templated_setup-0.959/templated_setup.egg-info/
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:29:51.000000 templated_setup-0.959/templated_setup.egg-info/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)      240 2024-05-02 09:29:52.000000 templated_setup-0.959/templated_setup.egg-info/SOURCES.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 09:29:51.000000 templated_setup-0.959/templated_setup.egg-info/dependency_links.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 09:29:51.000000 templated_setup-0.959/templated_setup.egg-info/top_level.txt
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:34:34.735397 templated_setup-0.960/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.960/LICENCE
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:34:34.734431 templated_setup-0.960/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.960/README.md
+-rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 09:34:34.735501 templated_setup-0.960/setup.cfg
+-rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.960/setup.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:34:34.731465 templated_setup-0.960/templated_setup/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    16765 2024-05-02 09:34:25.000000 templated_setup-0.960/templated_setup/__init__.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:34:34.733874 templated_setup-0.960/templated_setup.egg-info/
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:34:34.000000 templated_setup-0.960/templated_setup.egg-info/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)      210 2024-05-02 09:34:34.000000 templated_setup-0.960/templated_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 09:34:34.000000 templated_setup-0.960/templated_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 09:34:34.000000 templated_setup-0.960/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.959/LICENCE` & `templated_setup-0.960/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.959/PKG-INFO` & `templated_setup-0.960/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.959
+Version: 0.960
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
 
-## V0.959 released on 2nd/5/2024
+## V0.960 released on 2nd/5/2024
 god please kill me. ;(
```

### Comparing `templated_setup-0.959/README.md` & `templated_setup-0.960/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.959/templated_setup/__init__.py` & `templated_setup-0.960/templated_setup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,18 +572,16 @@
 		f"[ END ] {_Setup_Helper.init}"
 
 
 
 	@classmethod
 	def setup(cls, name:"str", author:"str", description:"str", **kwargs_for_setup_tools) -> "None":
 		
-
 		if cls._is_using_pip:
-			cls._name = name
-			cls._handle_installation_via_pip()
+			cls._handle_installation_via_pip(name)
 			return
 
 		_Setup_Helper.__clear_screen()
 
 		if not cls.__activated_already:
 			raise Exception("You must call `init` before calling `setup`.")
 
@@ -631,18 +629,19 @@
 	#################
 	# JUICY METHODS #
 	#################
 
 
 
 	@classmethod
-	def _handle_installation_via_pip(cls):
+	def _handle_installation_via_pip(cls, name):
 
 		setup(
-			name=cls._name,
+			name=name,
+			version="0.960"
 		)
 
 		return None
 	
 		f"[ END ] {_Setup_Helper._handle_installation_via_pip}"
```

### Comparing `templated_setup-0.959/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.960/templated_setup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.959
+Version: 0.960
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
 
-## V0.959 released on 2nd/5/2024
+## V0.960 released on 2nd/5/2024
 god please kill me. ;(
```

