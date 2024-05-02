# Comparing `tmp/templated_setup-0.963.tar.gz` & `tmp/templated_setup-0.964.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.963.tar", last modified: Thu May  2 09:52:50 2024, max compression
+gzip compressed data, was "templated_setup-0.964.tar", last modified: Thu May  2 10:10:35 2024, max compression
```

## Comparing `templated_setup-0.963.tar` & `templated_setup-0.964.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:52:50.839087 templated_setup-0.963/
--rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.963/LICENCE
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:52:50.838222 templated_setup-0.963/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.963/README.md
--rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 09:52:50.839226 templated_setup-0.963/setup.cfg
--rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.963/setup.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:52:50.801386 templated_setup-0.963/templated_setup/
--rw-r--r--   0 joel-watson   (501) staff       (20)    17346 2024-05-02 09:52:24.000000 templated_setup-0.963/templated_setup/__init__.py
--rw-r--r--   0 joel-watson   (501) staff       (20)       21 2024-05-02 09:52:49.000000 templated_setup-0.963/templated_setup/_hardcoded_version.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:52:50.837420 templated_setup-0.963/templated_setup.egg-info/
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:52:50.000000 templated_setup-0.963/templated_setup.egg-info/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)      248 2024-05-02 09:52:50.000000 templated_setup-0.963/templated_setup.egg-info/SOURCES.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 09:52:50.000000 templated_setup-0.963/templated_setup.egg-info/dependency_links.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 09:52:50.000000 templated_setup-0.963/templated_setup.egg-info/top_level.txt
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 10:10:35.345346 templated_setup-0.964/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.964/LICENCE
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 10:10:35.344725 templated_setup-0.964/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.964/README.md
+-rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 10:10:35.345459 templated_setup-0.964/setup.cfg
+-rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.964/setup.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 10:10:35.342454 templated_setup-0.964/templated_setup/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    17998 2024-05-02 10:10:08.000000 templated_setup-0.964/templated_setup/__init__.py
+-rw-r--r--   0 joel-watson   (501) staff       (20)       21 2024-05-02 10:10:35.000000 templated_setup-0.964/templated_setup/_hardcoded_version.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 10:10:35.344264 templated_setup-0.964/templated_setup.egg-info/
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 10:10:35.000000 templated_setup-0.964/templated_setup.egg-info/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)      248 2024-05-02 10:10:35.000000 templated_setup-0.964/templated_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 10:10:35.000000 templated_setup-0.964/templated_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 10:10:35.000000 templated_setup-0.964/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.963/LICENCE` & `templated_setup-0.964/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.963/PKG-INFO` & `templated_setup-0.964/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.963
+Version: 0.964
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
 
-## V0.963 released on 2nd/5/2024
+## V0.964 released on 2nd/5/2024
 god please kill me. ;(
```

### Comparing `templated_setup-0.963/README.md` & `templated_setup-0.964/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.963/templated_setup/__init__.py` & `templated_setup-0.964/templated_setup/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 By using this software, you, the user, acknowledge and agree that you are solely responsible for the content that is published using this tool.
 The software is provided "as is", and the developers make no representations or warranties of any kind regarding its use.
 
 You assume all responsibility and risk for the use of this software and the materials you create or publish with it.
 
 The developers shall not be liable for any claims, damages, or other liabilities arising from the use of the software or content published therein.
 
+-- END OF LEGAL NOTICE --
+
+NOTE: If you would like to remove this legal notice in future, simply set "_TEMPLATED_SETUP_PLEASE="STFU" as an environment variable.
+
 ========================
 THANK YOU AND TAKE CARE!
 ========================
 
 """
 
 
@@ -430,14 +434,20 @@
 
 		f"[ END ] {_Setup_Helper.__inner_load_readme_file_path}"
 
 
 
 	@classmethod
 	def __load_parameters(cls, force=False):
+		if not force and not cls._json_data:
+			try:
+				with open(CACHE_FILE_PATH, "r") as f:
+					cls._json_data = json_x_load(f)
+			except FileNotFoundError:
+				force = True
 		if not force:
 			cls.__load_cached_data()
 			cls.__load_date()
 			cls.__load_version_number()
 			cls.__load_notes()
 			cls.__load_readme_file_path()
 		user_wants_to_change_params = False
@@ -586,25 +596,37 @@
 			return
 
 		_Setup_Helper.__clear_screen()
 
 		if not cls.__activated_already:
 			raise Exception("You must call `init` before calling `setup`.")
 
-		for c in LEGAL_NOTICE:
-			print(c, end="", flush=True)
-			time_x_sleep(0.001)
-		print("\n")
-		time_x_sleep(0.5)
-		print(".", end="", flush=True)
-		time_x_sleep(0.5)
-		print(".", end="", flush=True)
-		time_x_sleep(0.5)
-		print(".", end="", flush=True)
-		time_x_sleep(0.8)
+		starting_i = 3
+		i = starting_i
+		do_print_legal_notice = True
+		if "_TEMPLATED_SETUP_PLEASE" in os.environ:
+			if os.environ["_TEMPLATED_SETUP_PLEASE"] == "STFU":
+				do_print_legal_notice = False
+		if do_print_legal_notice:
+			for c in LEGAL_NOTICE:
+				i -= 1
+				if i == 0:
+					i = starting_i
+					time_x_sleep(0.01)
+					print(c, end="", flush=True)
+				else:
+					print(c, end="")
+			print("\n")
+			time_x_sleep(0.5)
+			print(".", end="", flush=True)
+			time_x_sleep(0.5)
+			print(".", end="", flush=True)
+			time_x_sleep(0.5)
+			print(".", end="", flush=True)
+			time_x_sleep(0.8)
 
 		cls._name = name
 		cls._author = author
 		cls._description = description
 
 		_Setup_Helper.__load_parameters()
```

### Comparing `templated_setup-0.963/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.964/templated_setup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.963
+Version: 0.964
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
 
-## V0.963 released on 2nd/5/2024
+## V0.964 released on 2nd/5/2024
 god please kill me. ;(
```

