# Comparing `tmp/templated_setup-0.962.tar.gz` & `tmp/templated_setup-0.963.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.962.tar", last modified: Thu May  2 09:46:44 2024, max compression
+gzip compressed data, was "templated_setup-0.963.tar", last modified: Thu May  2 09:52:50 2024, max compression
```

## Comparing `templated_setup-0.962.tar` & `templated_setup-0.963.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:46:44.157474 templated_setup-0.962/
--rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.962/LICENCE
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:46:44.156451 templated_setup-0.962/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.962/README.md
--rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 09:46:44.157646 templated_setup-0.962/setup.cfg
--rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.962/setup.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:46:44.153161 templated_setup-0.962/templated_setup/
--rw-r--r--   0 joel-watson   (501) staff       (20)    17267 2024-05-02 09:45:41.000000 templated_setup-0.962/templated_setup/__init__.py
--rw-r--r--   0 joel-watson   (501) staff       (20)       21 2024-05-02 09:46:43.000000 templated_setup-0.962/templated_setup/_hardcoded_version.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:46:44.155791 templated_setup-0.962/templated_setup.egg-info/
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:46:44.000000 templated_setup-0.962/templated_setup.egg-info/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)      248 2024-05-02 09:46:44.000000 templated_setup-0.962/templated_setup.egg-info/SOURCES.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 09:46:44.000000 templated_setup-0.962/templated_setup.egg-info/dependency_links.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 09:46:44.000000 templated_setup-0.962/templated_setup.egg-info/top_level.txt
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:52:50.839087 templated_setup-0.963/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.963/LICENCE
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:52:50.838222 templated_setup-0.963/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.963/README.md
+-rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 09:52:50.839226 templated_setup-0.963/setup.cfg
+-rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.963/setup.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:52:50.801386 templated_setup-0.963/templated_setup/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    17346 2024-05-02 09:52:24.000000 templated_setup-0.963/templated_setup/__init__.py
+-rw-r--r--   0 joel-watson   (501) staff       (20)       21 2024-05-02 09:52:49.000000 templated_setup-0.963/templated_setup/_hardcoded_version.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:52:50.837420 templated_setup-0.963/templated_setup.egg-info/
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:52:50.000000 templated_setup-0.963/templated_setup.egg-info/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)      248 2024-05-02 09:52:50.000000 templated_setup-0.963/templated_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 09:52:50.000000 templated_setup-0.963/templated_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 09:52:50.000000 templated_setup-0.963/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.962/LICENCE` & `templated_setup-0.963/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.962/PKG-INFO` & `templated_setup-0.963/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.962
+Version: 0.963
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
 
-## V0.962 released on 2nd/5/2024
+## V0.963 released on 2nd/5/2024
 god please kill me. ;(
```

### Comparing `templated_setup-0.962/README.md` & `templated_setup-0.963/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.962/templated_setup/__init__.py` & `templated_setup-0.963/templated_setup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,14 +412,17 @@
 		f"[ END ] {_Setup_Helper.__load_readme_file_path}"
 
 
 
 	@classmethod
 	def __inner_load_readme_file_path(cls) -> "None":
 
+		assert cls._json_data
+		assert not cls._is_using_pip
+
 		cls._readme_file_path = _Setup_Helper.__get_answer(
 			"Enter the path to the README file: ",
 			lambda x: (os.path.exists(x), "File does not exist.")
 		)
 
 		cls._json_data["readme_file_path"] = cls._readme_file_path
 
@@ -546,14 +549,16 @@
 		cls._base_dir = os.path.abspath(cls._base_dir)
 
 		cls._date_of_last_modified = None
 		cls._version_number = None
 		cls._notes = None
 		cls._readme_file_path = None
 
+		cls._json_data = None
+
 		cls._is_using_pip = False
 		try:
 			print("] Press ENTER to continue...")
 			input()
 		except EOFError:
 			cls._is_using_pip = True
 		if "PIP_BUILD_TRACKER" in os.environ:
@@ -583,15 +588,15 @@
 		_Setup_Helper.__clear_screen()
 
 		if not cls.__activated_already:
 			raise Exception("You must call `init` before calling `setup`.")
 
 		for c in LEGAL_NOTICE:
 			print(c, end="", flush=True)
-			time_x_sleep(0.00075)
+			time_x_sleep(0.001)
 		print("\n")
 		time_x_sleep(0.5)
 		print(".", end="", flush=True)
 		time_x_sleep(0.5)
 		print(".", end="", flush=True)
 		time_x_sleep(0.5)
 		print(".", end="", flush=True)
```

### Comparing `templated_setup-0.962/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.963/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.962
+Version: 0.963
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
 
-## V0.962 released on 2nd/5/2024
+## V0.963 released on 2nd/5/2024
 god please kill me. ;(
```

