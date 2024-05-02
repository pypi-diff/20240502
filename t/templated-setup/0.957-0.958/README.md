# Comparing `tmp/templated_setup-0.957.tar.gz` & `tmp/templated_setup-0.958.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.957.tar", last modified: Thu May  2 09:16:20 2024, max compression
+gzip compressed data, was "templated_setup-0.958.tar", last modified: Thu May  2 09:27:43 2024, max compression
```

## Comparing `templated_setup-0.957.tar` & `templated_setup-0.958.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:16:20.341059 templated_setup-0.957/
--rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.957/LICENCE
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:16:20.339620 templated_setup-0.957/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.957/README.md
--rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 09:16:20.341266 templated_setup-0.957/setup.cfg
--rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.957/setup.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:16:20.334075 templated_setup-0.957/templated_setup/
--rw-r--r--   0 joel-watson   (501) staff       (20)    16973 2024-05-02 09:15:03.000000 templated_setup-0.957/templated_setup/__init__.py
--rw-r--r--   0 joel-watson   (501) staff       (20)      144 2024-05-02 09:03:39.000000 templated_setup-0.957/templated_setup/_hardcoded.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:16:20.338680 templated_setup-0.957/templated_setup.egg-info/
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:16:19.000000 templated_setup-0.957/templated_setup.egg-info/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)      240 2024-05-02 09:16:20.000000 templated_setup-0.957/templated_setup.egg-info/SOURCES.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 09:16:19.000000 templated_setup-0.957/templated_setup.egg-info/dependency_links.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 09:16:19.000000 templated_setup-0.957/templated_setup.egg-info/top_level.txt
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:27:43.449390 templated_setup-0.958/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.958/LICENCE
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:27:43.447929 templated_setup-0.958/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.958/README.md
+-rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 09:27:43.449592 templated_setup-0.958/setup.cfg
+-rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.958/setup.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:27:43.404693 templated_setup-0.958/templated_setup/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    16731 2024-05-02 09:26:55.000000 templated_setup-0.958/templated_setup/__init__.py
+-rw-r--r--   0 joel-watson   (501) staff       (20)      144 2024-05-02 09:03:39.000000 templated_setup-0.958/templated_setup/_hardcoded.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:27:43.408802 templated_setup-0.958/templated_setup.egg-info/
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:27:42.000000 templated_setup-0.958/templated_setup.egg-info/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)      240 2024-05-02 09:27:42.000000 templated_setup-0.958/templated_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 09:27:42.000000 templated_setup-0.958/templated_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 09:27:42.000000 templated_setup-0.958/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.957/LICENCE` & `templated_setup-0.958/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.957/PKG-INFO` & `templated_setup-0.958/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.957
+Version: 0.958
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
 
-## V0.957 released on 2nd/5/2024
+## V0.958 released on 2nd/5/2024
 god please kill me. ;(
```

### Comparing `templated_setup-0.957/README.md` & `templated_setup-0.958/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.957/templated_setup/__init__.py` & `templated_setup-0.958/templated_setup/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -555,14 +555,17 @@
 			print("] Press ENTER to continue...")
 			input()
 		except EOFError:
 			cls._is_using_pip = True
 		if "PIP_BUILD_TRACKER" in os.environ:
 			cls._is_using_pip = True
 
+		if cls._is_using_pip:
+			cls._handle_installation_via_pip()
+
 		try:
 			__ = cls.__activated_already
 		except AttributeError:
 			cls.__activated_already = None
 		if cls.__activated_already:
 			raise Exception("This class is a singleton and can only be activated once.")
 		cls.__activated_already = True
@@ -577,50 +580,46 @@
 	def setup(cls, name:"str", author:"str", description:"str", **kwargs_for_setup_tools) -> "None":
 		
 		_Setup_Helper.__clear_screen()
 
 		if not cls.__activated_already:
 			raise Exception("You must call `init` before calling `setup`.")
 
-		if not cls._is_using_pip:
-			for c in LEGAL_NOTICE:
-				print(c, end="", flush=True)
-				time_x_sleep(0.00075)
-			print("\n")
-			time_x_sleep(0.5)
-			print(".", end="", flush=True)
-			time_x_sleep(0.5)
-			print(".", end="", flush=True)
-			time_x_sleep(0.5)
-			print(".", end="", flush=True)
-			time_x_sleep(0.8)
-		else:
-			print("Running via pip.")
+		for c in LEGAL_NOTICE:
+			print(c, end="", flush=True)
+			time_x_sleep(0.00075)
+		print("\n")
+		time_x_sleep(0.5)
+		print(".", end="", flush=True)
+		time_x_sleep(0.5)
+		print(".", end="", flush=True)
+		time_x_sleep(0.5)
+		print(".", end="", flush=True)
+		time_x_sleep(0.8)
 
 		cls._name = name
 		cls._author = author
 		cls._description = description
 
-		if not cls._is_using_pip:
-			_Setup_Helper.__load_parameters()
+		_Setup_Helper.__load_parameters()
+
+		assert isinstance(cls._date_of_last_modified, str)
+		cls._date_of_last_modified = datetime_x_date.fromisoformat(cls._date_of_last_modified)
 
-			assert isinstance(cls._date_of_last_modified, str)
-			cls._date_of_last_modified = datetime_x_date.fromisoformat(cls._date_of_last_modified)
+		assert isinstance(cls._date_of_last_modified, datetime_x_date)
+		assert isinstance(cls._version_number, str)
+		assert isinstance(cls._notes, str)
+		assert isinstance(cls._readme_file_path, str)
 
-			assert isinstance(cls._date_of_last_modified, datetime_x_date)
-			assert isinstance(cls._version_number, str)
-			assert isinstance(cls._notes, str)
-			assert isinstance(cls._readme_file_path, str)
-
-			cls._version = _Version(
-				date=cls._date_of_last_modified,
-				version_number=cls._version_number,
-				notes=_Setup_Helper.__parse_notes(cls._notes)
-			)
-			cls._version.validate()
+		cls._version = _Version(
+			date=cls._date_of_last_modified,
+			version_number=cls._version_number,
+			notes=_Setup_Helper.__parse_notes(cls._notes)
+		)
+		cls._version.validate()
 
 		cls._finish_setup(kwargs_for_setup_tools)
 
 		return None
 
 		f"[ END ] {_Setup_Helper.setup}"
 
@@ -629,34 +628,42 @@
 	#################
 	# JUICY METHODS #
 	#################
 
 
 
 	@classmethod
+	def _handle_installation_via_pip(cls):
+
+		setup(
+			name=cls._name,
+		)
+
+		return None
+	
+		f"[ END ] {_Setup_Helper._handle_installation_via_pip}"
+
+
+
+	@classmethod
 	def _finish_setup(cls, kwargs_for_setup_tools:"dict"):
 
 		assert isinstance(cls._date_of_last_modified, datetime_x_date)
 		assert isinstance(cls._version_number, str)
 		assert isinstance(cls._notes, str)
 		assert isinstance(cls._readme_file_path, str)
 
 		long_description = _Setup_Helper.__init_description(cls._readme_file_path)
 		long_description += f"\n## V{cls._version.version_number} released on {cls._version.repr_date()}\n"
 		long_description += cls._notes
 
-		if not cls._is_using_pip:
-			_Setup_Helper.__clear_screen()
-			print(f"Current Directory: [{os.path.abspath(os.getcwd())}].\n\n")
-			is_root_of_project = _Setup_Helper.__get_y_n("Is this the root of the project?")
-			_Setup_Helper.__clear_screen()
-		else:
-			if not os.path.exists(os.path.join(cls._base_dir, "..", "setup.py")):
-				raise FileNotFoundError("The `setup.py` file does not exist. Please run this script from the root of the project directory.")
-			is_root_of_project = True
+		_Setup_Helper.__clear_screen()
+		print(f"Current Directory: [{os.path.abspath(os.getcwd())}].\n\n")
+		is_root_of_project = _Setup_Helper.__get_y_n("Is this the root of the project?")
+		_Setup_Helper.__clear_screen()
 
 		if not is_root_of_project:
 			raise Exception("This script must be run from the root of the project directory.")
 		
 		dirs_to_remove = [
 			"dist",
 			"build",
@@ -672,36 +679,32 @@
 						time_x_sleep(3)
 						shutil.rmtree(d, ignore_errors=True)
 			except KeyboardInterrupt:
 				print("] Cancelled.")
 				exit(0)
 			_Setup_Helper.__clear_screen()
 
-		if not cls._is_using_pip:
-			cls._old_sys_argv = sys.argv
-			sys.argv = [sys.argv[0], "sdist"]
-			do_proceed = _Setup_Helper.__get_y_n("Would you like to proceed with the build?")
-			if not do_proceed:
-				exit(0)
-			_Setup_Helper.__clear_screen()
+		cls._old_sys_argv = sys.argv
+		sys.argv = [sys.argv[0], "sdist"]
+		do_proceed = _Setup_Helper.__get_y_n("Would you like to proceed with the build?")
+		if not do_proceed:
+			exit(0)
+		_Setup_Helper.__clear_screen()
 
 		setup(
 			name=cls._name,
 			version=cls._version.version_number,
 			author=cls._author,
 			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
 			long_description=long_description,
 			**kwargs_for_setup_tools,
 		)
 
-		if not cls._is_using_pip:
-			print("\n] Setup complete.\n\n")
-		else:
-			return
+		print("\n] Setup complete.\n\n")
 
 		do_publish = _Setup_Helper.__get_y_n("Would you like to publish to PyPi?")
 		if not do_publish:
 			exit(0)
 
 		_Setup_Helper.__clear_screen()
```

### Comparing `templated_setup-0.957/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.958/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.957
+Version: 0.958
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
 
-## V0.957 released on 2nd/5/2024
+## V0.958 released on 2nd/5/2024
 god please kill me. ;(
```

