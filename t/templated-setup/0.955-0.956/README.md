# Comparing `tmp/templated_setup-0.955.tar.gz` & `tmp/templated_setup-0.956.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.955.tar", last modified: Thu May  2 08:40:43 2024, max compression
+gzip compressed data, was "templated_setup-0.956.tar", last modified: Thu May  2 09:09:58 2024, max compression
```

## Comparing `templated_setup-0.955.tar` & `templated_setup-0.956.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 08:40:43.622304 templated_setup-0.955/
--rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.955/LICENCE
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 08:40:43.621022 templated_setup-0.955/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.955/README.md
--rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 08:40:43.622483 templated_setup-0.955/setup.cfg
--rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.955/setup.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 08:40:43.579068 templated_setup-0.955/templated_setup/
--rw-r--r--   0 joel-watson   (501) staff       (20)    20222 2024-05-02 08:39:32.000000 templated_setup-0.955/templated_setup/__init__.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 08:40:43.620134 templated_setup-0.955/templated_setup.egg-info/
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 08:40:42.000000 templated_setup-0.955/templated_setup.egg-info/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)      210 2024-05-02 08:40:43.000000 templated_setup-0.955/templated_setup.egg-info/SOURCES.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 08:40:42.000000 templated_setup-0.955/templated_setup.egg-info/dependency_links.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 08:40:42.000000 templated_setup-0.955/templated_setup.egg-info/top_level.txt
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:09:58.574413 templated_setup-0.956/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.956/LICENCE
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:09:58.573416 templated_setup-0.956/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.956/README.md
+-rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 09:09:58.574569 templated_setup-0.956/setup.cfg
+-rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.956/setup.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:09:58.569297 templated_setup-0.956/templated_setup/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    16859 2024-05-02 09:08:52.000000 templated_setup-0.956/templated_setup/__init__.py
+-rw-r--r--   0 joel-watson   (501) staff       (20)      144 2024-05-02 09:03:39.000000 templated_setup-0.956/templated_setup/_hardcoded.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:09:58.572342 templated_setup-0.956/templated_setup.egg-info/
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:09:58.000000 templated_setup-0.956/templated_setup.egg-info/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)      240 2024-05-02 09:09:58.000000 templated_setup-0.956/templated_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 09:09:58.000000 templated_setup-0.956/templated_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 09:09:58.000000 templated_setup-0.956/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.955/LICENCE` & `templated_setup-0.956/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.955/PKG-INFO` & `templated_setup-0.956/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.955
+Version: 0.956
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
 
-## V0.955 released on 2nd/5/2024
+## V0.956 released on 2nd/5/2024
 god please kill me. ;(
```

### Comparing `templated_setup-0.955/README.md` & `templated_setup-0.956/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.955/templated_setup/__init__.py` & `templated_setup-0.956/templated_setup/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -207,54 +207,44 @@
 
 		return None
 		f"[ END ] {_Setup_Helper.__get_y_n}"
 
 
 
 	@classmethod
-	def __inner_reload_cached_data(cls):
+	def __load_cached_data(cls):
 
 		try:
 			with open(CACHE_FILE_PATH, "r") as f:
 				json_data = json_x_load(f)
 		except FileNotFoundError:
-			if cls._json_data and len(cls._json_data.keys()) == 0:
-				if cls._is_using_pip:
-					return
+			if cls._json_data and len(cls._json_data.keys()) > 0:
+				with open(CACHE_FILE_PATH, "w") as f:
+					json_x_dump(cls._json_data, f)
+			else:
 				with open(CACHE_FILE_PATH, "w") as f:
 					json_x_dump({}, f)
 				with open(CACHE_FILE_PATH, "r") as f:
 					json_data = json_x_load(f)
-			else:
-				return
 
 		cls._json_data = json_data
 
 		return None
 
 		f"[ END ] {_Setup_Helper.__reload_cached_data}"
 
 
-	
-	@classmethod
-	def __reload_cached_data(cls):
-		cls._load_from_hardcoded()
-		return None
-		f"[ END ] {_Setup_Helper.__reload_cached_data}"
-
-
 
 	@classmethod
-	def __load_date(cls, override=False):
-
-		if cls._date_of_last_modified:
-			cls.__reload_cached_data()
+	def __load_date(cls, override=False) -> "None":
+		
+		assert cls._json_data
+		assert not cls._is_using_pip
 
-		if not cls._is_using_pip and not override and cls._json_data is not None:
-			assert cls._json_data
+		if not override:
 			if "date" in cls._json_data:
 				cls._date_of_last_modified = datetime_x_date.fromisoformat(cls._json_data["date"])
 			else:
 				while True:
 					new = cls.__inner_load_date()
 					confirmed = _Setup_Helper.__get_y_n(f"Is [{new}] Correct?")
 					if confirmed:
@@ -266,25 +256,23 @@
 		return None
 
 		f"[ END ] {_Setup_Helper.__load_date}"
 
 
 
 	@classmethod
-	def __inner_load_date(cls) -> "str":
-		if cls._is_using_pip:
-			cls._date_of_last_modified = datetime_x_date.today()
-			return cls._date_of_last_modified.isoformat()
+	def __inner_load_date(cls) -> "None":
+		assert cls._json_data
+		assert not cls._is_using_pip
 		do_want_to_use_current_date = _Setup_Helper.__get_y_n("Would you like to use the current date?")
 		new = None
 		if do_want_to_use_current_date:
 
 			cls._date_of_last_modified = datetime_x_date.today()
-			if cls._json_data:
-				cls._json_data["date"] = cls._date_of_last_modified.isoformat()
+			cls._json_data["date"] = cls._date_of_last_modified.isoformat()
 			new = cls._date_of_last_modified.isoformat()
 
 		else:
 
 			day = int(_Setup_Helper.__get_answer(
 				"What day was it last modified? ",
 				lambda x: (x.isdigit(), "Please enter a number."))
@@ -301,35 +289,31 @@
 			)
 
 			try:
 				cls._date_of_last_modified = datetime_x_date(year, month, day)
 				assert cls._json_data
 				cls._json_data["date"] = cls._date_of_last_modified.isoformat()
 				new = cls._date_of_last_modified.isoformat()
-
 			except ValueError:
 				print("] Error: Invalid date. Please try again.")
 		
-		if cls._json_data is not None:
-			with open(CACHE_FILE_PATH, "w") as f:
-				json_x_dump(cls._json_data, f)
-		assert isinstance(new, str)
-		return new
+		assert isinstance(cls._date_of_last_modified, str)
+		cls._date_of_last_modified = new
+		return None
 		f"[ END ] {_Setup_Helper.__inner_load_date}"
 
 
 
 	@classmethod
-	def __load_version_number(cls, override=False):
+	def __load_version_number(cls, override=False) -> "None":
 
-		if cls._version_number:
-			cls.__reload_cached_data()
+		assert cls._json_data
+		assert not cls._is_using_pip
 
-		if not cls._is_using_pip and not override:
-			assert cls._json_data
+		if not override:
 			if "version_number" in cls._json_data:
 				cls._version_number = cls._json_data["version_number"]
 			else:
 				while True:
 					new = cls.__inner_load_version_number()
 					confirmed = _Setup_Helper.__get_y_n(f"Is [{new}] Correct?")
 					if confirmed:
@@ -340,44 +324,39 @@
 		return None
 	
 		f"[ END ] {_Setup_Helper.__load_version_number}"
 
 
 
 	@classmethod
-	def __inner_load_version_number(cls) -> "str":
+	def __inner_load_version_number(cls) -> "None":
 
-		if cls._is_using_pip:
-			cls._version_number = "0.0"
-			return cls._version_number		
+		assert cls._json_data
+		assert not cls._is_using_pip
 
 		cls._version_number = _Setup_Helper.__get_answer(
 			"What is the version number? ",
 			_Version.validate_version_number
 		)
 
-		if cls._json_data:
-			cls._json_data["version_number"] = cls._version_number
+		cls._json_data["version_number"] = cls._version_number
 
-		if cls._json_data is not None:
-			with open(CACHE_FILE_PATH, "w") as f:
-				json_x_dump(cls._json_data, f)
-
-		return cls._version_number
+		return None
 
 		f"[ END ] {_Setup_Helper.__inner_load_version_number}"
 
 
 
 	@classmethod
-	def __load_notes(cls, override=False):
+	def __load_notes(cls, override=False) -> "None":
 
+		assert cls._json_data
+		assert not cls._is_using_pip
 
-		if not cls._is_using_pip and not override:
-			assert cls._json_data
+		if not override:
 			if "notes" in cls._json_data:
 				cls._notes = cls._json_data["notes"]
 			else:
 				while True:
 					new = cls.__inner_load_notes()
 					confirmed = _Setup_Helper.__get_y_n(f"Is [{new}] Correct?")
 					if confirmed:
@@ -388,47 +367,39 @@
 		return None
 
 		f"[ END ] {_Setup_Helper.__load_notes}"
 
 
 
 	@classmethod
-	def __inner_load_notes(cls) -> "str":
+	def __inner_load_notes(cls) -> "None":
 		
-		if cls._is_using_pip:
-			cls._notes = "No notes."
-			return cls._notes
+		assert cls._json_data
+		assert not cls._is_using_pip
 
 		cls._notes = _Setup_Helper.__get_answer(
 			"Enter the release notes: ",
 			lambda x: (len(x) > 0, "Notes cannot be empty.")
 		)
 
-		if cls._json_data:
-			cls._json_data["notes"] = cls._notes
-
-		if cls._json_data is not None:
-			with open(CACHE_FILE_PATH, "w") as f:
-				json_x_dump(cls._json_data, f)
+		cls._json_data["notes"] = cls._notes
 
-		return cls._notes
+		return None
 
 		f"[ END ] {_Setup_Helper.__inner_load_notes}"
 
 
 
 	@classmethod
-	def __load_readme_file_path(cls, override=False):
+	def __load_readme_file_path(cls, override=False) -> "None":
 		
-		if cls._readme_file_path:
-			cls._readme_file_path = "README.md"
-			return
+		assert cls._json_data
+		assert not cls._is_using_pip
 
 		if not override:
-			assert cls._json_data
 			if "readme_file_path" in cls._json_data:
 				cls._readme_file_path = cls._json_data["readme_file_path"]
 			else:
 				while True:
 					new = cls.__inner_load_readme_file_path()
 					confirmed = _Setup_Helper.__get_y_n(f"Is [{new}] Correct?")
 					if confirmed:
@@ -439,46 +410,37 @@
 		return None
 
 		f"[ END ] {_Setup_Helper.__load_readme_file_path}"
 
 
 
 	@classmethod
-	def __inner_load_readme_file_path(cls) -> "str":
+	def __inner_load_readme_file_path(cls) -> "None":
 
 		cls._readme_file_path = _Setup_Helper.__get_answer(
 			"Enter the path to the README file: ",
 			lambda x: (os.path.exists(x), "File does not exist.")
 		)
 
-		if cls._json_data:
-			cls._json_data["readme_file_path"] = cls._readme_file_path
+		cls._json_data["readme_file_path"] = cls._readme_file_path
 
-		if cls._json_data is not None:
-			with open(CACHE_FILE_PATH, "w") as f:
-				json_x_dump(cls._json_data, f)
-
-		return cls._readme_file_path
+		return None
 
 		f"[ END ] {_Setup_Helper.__inner_load_readme_file_path}"
 
 
 
 	@classmethod
 	def __load_parameters(cls, force=False):
-		if cls._is_using_pip:
-			json_data = cls._json_data_when_using_pip
-			assert json_data is not None
-			cls._date_of_last_modified = datetime_x_date.fromisoformat(json_data["date"])
-			cls._version_number = json_data["version_number"]
-			cls._notes = json_data["notes"]
-			cls._readme_file_path = json_data["readme_file_path"]
-			return
 		if not force:
-			cls.__inner_reload_cached_data()
+			cls.__load_cached_data()
+			cls.__load_date()
+			cls.__load_version_number()
+			cls.__load_notes()
+			cls.__load_readme_file_path()
 		user_wants_to_change_params = False
 		if force:
 			user_wants_to_change_params = True
 		while True:
 
 			cls.__clear_screen()
 			print(f"\n\n] Current Infos:")
@@ -508,23 +470,27 @@
 					)
 				))
 				if choice == len(options)+1:
 					user_wants_to_change_params = False
 					continue
 				callback = options[choice-1][1]
 				callback()
+				with open(CACHE_FILE_PATH, "w") as f:
+					json_x_dump(cls._json_data, f)
+				cls.__load_cached_data()
 				continue
 
 			if force:
 				assert cls._date_of_last_modified
 				assert cls._version_number
 				assert cls._notes
 				assert cls._readme_file_path
+				assert not cls._json_data
 				json_data = {}
-				json_data["date"] = cls._date_of_last_modified.isoformat()
+				json_data["date"] = cls._date_of_last_modified
 				json_data["version_number"] = cls._version_number
 				json_data["notes"] = cls._notes
 				json_data["readme_file_path"] = cls._readme_file_path
 				with open(CACHE_FILE_PATH, "w") as f:
 					json_x_dump(json_data, f)
 				cls.__clear_screen()
 				break
@@ -580,94 +546,34 @@
 		cls._base_dir = os.path.abspath(cls._base_dir)
 
 		cls._date_of_last_modified = None
 		cls._version_number = None
 		cls._notes = None
 		cls._readme_file_path = None
 
-		try:
-			__ = cls.__activated_already
-		except AttributeError:
-			cls.__activated_already = None
-		if cls.__activated_already:
-			raise Exception("This class is a singleton and can only be activated once.")
-		cls.__activated_already = True
-
-		cls._load_from_hardcoded()
-
-		return None
-	
-		f"[ END ] {_Setup_Helper.init}"
-
-
-
-	@classmethod
-	def _load_from_hardcoded(cls):
-
 		cls._is_using_pip = False
 		try:
+			print("] Press ENTER to continue...")
 			input()
 		except EOFError:
 			cls._is_using_pip = True
-		if "PIP_BUILD_TRACKER" in " ".join(os.environ.keys()):
+		if "PIP_BUILD_TRACKER" in os.environ:
 			cls._is_using_pip = True
 
 		try:
-			__ = cls._json_data
+			__ = cls.__activated_already
 		except AttributeError:
-			cls._json_data = None
-		cls.__inner_reload_cached_data()
-		json_data = {} if not cls._json_data else cls._json_data
-		needs_update = False
-
-		# Before uploading to PyPi, we need to hardcode the values in a source file.
-		try:
-			from . import _hardcoded #type:ignore
-		except ImportError:
-			if not json_data:
-				cls.__load_parameters(force=True)
-			with open(os.path.join(cls._base_dir, "_hardcoded.py"), "w") as f:
-				f.write(f"\"\"\"\n{json_x_dumps(json_data)}\n\"\"\"\n")
-			from . import _hardcoded #type:ignore
-		with open(_hardcoded.__file__, "r") as f:
-			contents = f.read()
-			splitted = contents.split("\n")[1:-2]
-			json_str = "\n".join(splitted)
-			j_data = json_x_loads(json_str)
-			if j_data != json_data:
-				needs_update = True
-		if needs_update and len(json_data.keys()) == 4:
-			with open(_hardcoded.__file__, "w") as f:
-				json_str = json_x_dumps(json_data, indent=4)
-				f.write(f"\"\"\"\n{json_str}\n\"\"\"\n")
-		with open(_hardcoded.__file__, "r") as f:
-			contents = f.read()
-			splitted = contents.split("\n")[1:-2]
-			json_str = "\n".join(splitted)
-			json_data = json_x_loads(json_str)
-
-		assert json_data is not None
-		cls._json_data = json_data
-
-		if cls._is_using_pip:
-			cls._json_data_when_using_pip = json_data
-			return None
-
-		if not json_data:
-			assert cls._json_data is not None
-			j_data = cls._json_data
-
-		cls._date_of_last_modified = datetime_x_date.fromisoformat(j_data.get("date", None))
-		cls._version_number = j_data.get("version_number", None)
-		cls._notes = j_data.get("notes", None)
-		cls._readme_file_path = j_data.get("readme_file_path", None)
+			cls.__activated_already = None
+		if cls.__activated_already:
+			raise Exception("This class is a singleton and can only be activated once.")
+		cls.__activated_already = True
 
 		return None
 	
-		f"[ END ] {_Setup_Helper._load_from_hardcoded}"
+		f"[ END ] {_Setup_Helper.init}"
 
 
 
 	@classmethod
 	def setup(cls, name:"str", author:"str", description:"str", **kwargs_for_setup_tools) -> "None":
 		
 		_Setup_Helper.__clear_screen()
@@ -686,44 +592,33 @@
 			print(".", end="", flush=True)
 			time_x_sleep(0.5)
 			print(".", end="", flush=True)
 			time_x_sleep(0.8)
 		else:
 			print("Running via pip.")
 
-
 		cls._name = name
 		cls._author = author
 		cls._description = description
 
-		_Setup_Helper.__load_parameters()
-		assert isinstance(cls._date_of_last_modified, datetime_x_date)
-		assert isinstance(cls._version_number, str)
-		assert isinstance(cls._notes, str)
-		assert isinstance(cls._readme_file_path, str)
-
-		cls._version = _Version(
-			date=cls._date_of_last_modified,
-			version_number=cls._version_number,
-			notes=_Setup_Helper.__parse_notes(cls._notes)
-		)
-		cls._version.validate()
+		if not cls._is_using_pip:
+			_Setup_Helper.__load_parameters()
+			assert isinstance(cls._date_of_last_modified, datetime_x_date)
+			assert isinstance(cls._version_number, str)
+			assert isinstance(cls._notes, str)
+			assert isinstance(cls._readme_file_path, str)
+
+			cls._version = _Version(
+				date=cls._date_of_last_modified,
+				version_number=cls._version_number,
+				notes=_Setup_Helper.__parse_notes(cls._notes)
+			)
+			cls._version.validate()
 
-		prev_hardcoded = None
-		try:
-			with open(os.path.join(cls._base_dir, "_hardcoded.py"), "r") as f:
-				prev_hardcoded = f.read()
-			if not prev_hardcoded:
-				raise Exception("The `_hardcoded.py` file is empty. Please run the script again.")
-			os.remove(os.path.join(cls._base_dir, "_hardcoded.py"))
-			cls._finish_setup(kwargs_for_setup_tools)
-		finally:
-			assert prev_hardcoded
-			with open(os.path.join(cls._base_dir, "_hardcoded.py"), "w") as f:
-				f.write(prev_hardcoded)
+		cls._finish_setup(kwargs_for_setup_tools)
 
 		return None
 
 		f"[ END ] {_Setup_Helper.setup}"
 
 
 
@@ -812,17 +707,14 @@
 
 		do_proceed = _Setup_Helper.__get_y_n("Would you like to proceed?")
 		if not do_proceed:
 			exit(0)
 
 		_Setup_Helper.__clear_screen()
 
-		# It would be very bad if we shipped the cache file with this package.
-		with open(os.path.join(cls._base_dir, "_hardcoded.py"), "w") as f:
-			f.write("\"\"\"\n{}\n\"\"\"\n")
 		os.system(f"{sys.executable} -m twine upload --verbose --repository pypi dist/*")
 
 		sys.argv = cls._old_sys_argv
 
 		return None
 	
 		f"[ END ] {_Setup_Helper._finish_setup}"
```

### Comparing `templated_setup-0.955/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.956/templated_setup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.955
+Version: 0.956
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
 
-## V0.955 released on 2nd/5/2024
+## V0.956 released on 2nd/5/2024
 god please kill me. ;(
```

