# Comparing `tmp/templated_setup-0.92.tar.gz` & `tmp/templated_setup-0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.92.tar", last modified: Thu May  2 02:21:24 2024, max compression
+gzip compressed data, was "templated_setup-0.93.tar", last modified: Thu May  2 04:37:21 2024, max compression
```

## Comparing `templated_setup-0.92.tar` & `templated_setup-0.93.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 02:21:24.991720 templated_setup-0.92/
--rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.92/LICENCE
--rw-r--r--   0 joel-watson   (501) staff       (20)     2465 2024-05-02 02:21:24.990052 templated_setup-0.92/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.92/README.md
--rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 02:21:24.992028 templated_setup-0.92/setup.cfg
--rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 02:18:46.000000 templated_setup-0.92/setup.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 02:21:24.948526 templated_setup-0.92/templated_setup/
--rw-r--r--   0 joel-watson   (501) staff       (20)    20070 2024-05-02 02:20:47.000000 templated_setup-0.92/templated_setup/__init__.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 02:21:24.950940 templated_setup-0.92/templated_setup.egg-info/
--rw-r--r--   0 joel-watson   (501) staff       (20)     2465 2024-05-02 02:21:24.000000 templated_setup-0.92/templated_setup.egg-info/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)      210 2024-05-02 02:21:24.000000 templated_setup-0.92/templated_setup.egg-info/SOURCES.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 02:21:24.000000 templated_setup-0.92/templated_setup.egg-info/dependency_links.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 02:21:24.000000 templated_setup-0.92/templated_setup.egg-info/top_level.txt
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 04:37:21.635780 templated_setup-0.93/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.93/LICENCE
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2465 2024-05-02 04:37:21.635308 templated_setup-0.93/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.93/README.md
+-rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 04:37:21.635869 templated_setup-0.93/setup.cfg
+-rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:31:02.000000 templated_setup-0.93/setup.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 04:37:21.633247 templated_setup-0.93/templated_setup/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    19909 2024-05-02 04:36:57.000000 templated_setup-0.93/templated_setup/__init__.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 04:37:21.634927 templated_setup-0.93/templated_setup.egg-info/
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2465 2024-05-02 04:37:21.000000 templated_setup-0.93/templated_setup.egg-info/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)      210 2024-05-02 04:37:21.000000 templated_setup-0.93/templated_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 04:37:21.000000 templated_setup-0.93/templated_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 04:37:21.000000 templated_setup-0.93/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.92/LICENCE` & `templated_setup-0.93/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.92/PKG-INFO` & `templated_setup-0.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.92
+Version: 0.93
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
 
-## V0.92 released on 2nd/5/2024
+## V0.93 released on 2nd/5/2024
 god please kill me. ;(
```

### Comparing `templated_setup-0.92/README.md` & `templated_setup-0.93/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.92/templated_setup/__init__.py` & `templated_setup-0.93/templated_setup/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -527,25 +527,25 @@
 
 				confirmed = _Setup_Helper.__get_y_n("Is this information correct?")
 				if confirmed:
 					break
 				else:
 					user_wants_to_change_params = True
 					print("] Error: Please enter the information again.")
-					time_x_sleep(0.8)
 					cls.__clear_screen()
 
 		return None
 	
 		f"[ END ] {_Setup_Helper.__load_parameters}"
 
 
 
 	@staticmethod
 	def __clear_screen():
+		time_x_sleep(1)
 		if os.name == "nt":
 
 			os.system("cls")
 
 		else:
 
 			os.system("clear")
@@ -561,15 +561,18 @@
 	
 
 
 	@classmethod
 	def init(cls, cache_file_path_:"str") -> "None":
 
 		global CACHE_FILE_PATH
-		CACHE_FILE_PATH = cache_file_path_
+		CACHE_FILE_PATH = os.path.abspath(cache_file_path_)
+
+		cls._base_dir = os.path.dirname(__file__)
+		cls._base_dir = os.path.abspath(cls._base_dir)
 
 		cls._date_of_last_modified = None
 		cls._version_number = None
 		cls._notes = None
 		cls._readme_file_path = None
 
 		try:
@@ -588,14 +591,17 @@
 
 
 
 	@classmethod
 	def _load_from_hardcoded(cls):
 
 		cls._is_using_pip = False
+		if "VIRTUAL_ENV" in os.environ.keys():
+			if "pip" in ' '.join(sys.argv):
+				cls._is_using_pip = True
 		if "PIP_BUILD_TRACKER" in os.environ.keys():
 			cls._is_using_pip = True
 
 		try:
 			__ = cls._json_data
 		except AttributeError:
 			cls._json_data = None
@@ -605,17 +611,15 @@
 
 		# Before uploading to PyPi, we need to hardcode the values in a source file.
 		try:
 			from . import _hardcoded #type:ignore
 		except ImportError:
 			if not json_data:
 				cls.__load_parameters(force=True)
-			base_dir = os.path.dirname(__file__)
-			base_dir = os.path.abspath(base_dir)
-			with open(os.path.join(base_dir, "_hardcoded.py"), "w") as f:
+			with open(os.path.join(cls._base_dir, "_hardcoded.py"), "w") as f:
 				f.write(f"\"\"\"\n{json_x_dumps(json_data)}\n\"\"\"\n")
 			from . import _hardcoded
 		with open(_hardcoded.__file__, "r") as f:
 			contents = f.read()
 			splitted = contents.split("\n")[1:-2]
 			json_str = "\n".join(splitted)
 			j_data = json_x_loads(json_str)
@@ -625,15 +629,14 @@
 			with open(_hardcoded.__file__, "w") as f:
 				json_str = json_x_dumps(json_data, indent=4)
 				f.write(f"\"\"\"\n{json_str}\n\"\"\"\n")
 		with open(_hardcoded.__file__, "r") as f:
 			contents = f.read()
 			splitted = contents.split("\n")[1:-2]
 			json_str = "\n".join(splitted)
-			print(json_str)
 			json_data = json_x_loads(json_str)
 
 		assert json_data is not None
 		cls._json_data = json_data
 
 		if cls._is_using_pip:
 			cls._json_data_when_using_pip = json_data
@@ -670,14 +673,16 @@
 			time_x_sleep(0.5)
 			print(".", end="", flush=True)
 			time_x_sleep(0.5)
 			print(".", end="", flush=True)
 			time_x_sleep(0.5)
 			print(".", end="", flush=True)
 			time_x_sleep(0.8)
+		else:
+			print("Running via pip.")
 
 
 		cls._name = name
 		cls._author = author
 		cls._description = description
 
 		_Setup_Helper.__load_parameters()
@@ -691,23 +696,23 @@
 			version_number=cls._version_number,
 			notes=_Setup_Helper.__parse_notes(cls._notes)
 		)
 		cls._version.validate()
 
 		prev_hardcoded = None
 		try:
-			with open(os.path.join(os.path.dirname(__file__), "_hardcoded.py"), "r") as f:
+			with open(os.path.join(cls._base_dir, "_hardcoded.py"), "r") as f:
 				prev_hardcoded = f.read()
 			if not prev_hardcoded:
 				raise Exception("The `_hardcoded.py` file is empty. Please run the script again.")
-			os.remove(os.path.join(os.path.dirname(__file__), "_hardcoded.py"))
+			os.remove(os.path.join(cls._base_dir, "_hardcoded.py"))
 			cls._finish_setup(kwargs_for_setup_tools)
 		finally:
 			assert prev_hardcoded
-			with open(os.path.join(os.path.dirname(__file__), "_hardcoded.py"), "w") as f:
+			with open(os.path.join(cls._base_dir, "_hardcoded.py"), "w") as f:
 				f.write(prev_hardcoded)
 
 		return None
 
 		f"[ END ] {_Setup_Helper.setup}"
 
 
@@ -733,36 +738,32 @@
 
 		if not cls._is_using_pip:
 			_Setup_Helper.__clear_screen()
 			print(f"Current Directory: [{os.path.abspath(os.getcwd())}].\n\n")
 			is_root_of_project = _Setup_Helper.__get_y_n("Is this the root of the project?")
 			_Setup_Helper.__clear_screen()
 		else:
-			if not os.path.exists("setup.py"):
+			if not os.path.exists(os.path.join(cls._base_dir, "..", "setup.py")):
 				raise FileNotFoundError("The `setup.py` file does not exist. Please run this script from the root of the project directory.")
-			if not os.path.exists("templated_setup/_hardcoded.py"):
-				raise FileNotFoundError("The `_hardcoded.py` file does not exist. Please run this script from the root of the project directory.")
 			is_root_of_project = True
 
 		if not is_root_of_project:
 			raise Exception("This script must be run from the root of the project directory.")
 		
-		separator = "\\" if os.name == "nt" else "/"
-
 		dirs_to_remove = [
 			"dist",
 			"build",
 			f"{cls._name}.egg-info"
 		]
 
 		if not cls._is_using_pip:
 			try:
 				for d in dirs_to_remove:
 					if os.path.exists(d):
-						print(f"\n] WARNING: ABOUT TO REMOVE THE `{os.getcwd()}{separator}{d}` DIRECTORY!!")
+						print(f"\n] WARNING: ABOUT TO REMOVE THE `{os.path.join(os.getcwd(),d)}` DIRECTORY!!")
 						print("] YOU HAVE 3 SECONDS TO CANCEL...")
 						time_x_sleep(3)
 						shutil.rmtree(d, ignore_errors=True)
 			except KeyboardInterrupt:
 				print("] Cancelled.")
 				exit(0)
 			_Setup_Helper.__clear_screen()
@@ -802,19 +803,16 @@
 		do_proceed = _Setup_Helper.__get_y_n("Would you like to proceed?")
 		if not do_proceed:
 			exit(0)
 
 		_Setup_Helper.__clear_screen()
 
 		# It would be very bad if we shipped the cache file with this package.
-		base_dir = os.path.dirname(__file__)
-		base_dir = os.path.abspath(base_dir)
-		with open(os.path.join(base_dir, "_hardcoded.py"), "w") as f:
+		with open(os.path.join(cls._base_dir, "_hardcoded.py"), "w") as f:
 			f.write("\"\"\"\n{}\n\"\"\"\n")
-
 		os.system(f"{sys.executable} -m twine upload --verbose --repository pypi dist/*")
 
 		sys.argv = cls._old_sys_argv
 
 		return None
 	
 		f"[ END ] {_Setup_Helper._finish_setup}"
```

### Comparing `templated_setup-0.92/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.93/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.92
+Version: 0.93
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
 
-## V0.92 released on 2nd/5/2024
+## V0.93 released on 2nd/5/2024
 god please kill me. ;(
```

