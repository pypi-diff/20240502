# Comparing `tmp/templated_setup-0.965.tar.gz` & `tmp/templated_setup-0.967.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.965.tar", last modified: Thu May  2 10:13:33 2024, max compression
+gzip compressed data, was "templated_setup-0.967.tar", last modified: Thu May  2 10:16:17 2024, max compression
```

## Comparing `templated_setup-0.965.tar` & `templated_setup-0.967.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 10:13:33.683217 templated_setup-0.965/
--rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.965/LICENCE
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 10:13:33.682620 templated_setup-0.965/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.965/README.md
--rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 10:13:33.683322 templated_setup-0.965/setup.cfg
--rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.965/setup.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 10:13:33.680178 templated_setup-0.965/templated_setup/
--rw-r--r--   0 joel-watson   (501) staff       (20)    18060 2024-05-02 10:12:49.000000 templated_setup-0.965/templated_setup/__init__.py
--rw-r--r--   0 joel-watson   (501) staff       (20)       21 2024-05-02 10:13:33.000000 templated_setup-0.965/templated_setup/_hardcoded_version.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 10:13:33.681983 templated_setup-0.965/templated_setup.egg-info/
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 10:13:33.000000 templated_setup-0.965/templated_setup.egg-info/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)      248 2024-05-02 10:13:33.000000 templated_setup-0.965/templated_setup.egg-info/SOURCES.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 10:13:33.000000 templated_setup-0.965/templated_setup.egg-info/dependency_links.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 10:13:33.000000 templated_setup-0.965/templated_setup.egg-info/top_level.txt
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 10:16:17.545325 templated_setup-0.967/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.967/LICENCE
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2477 2024-05-02 10:16:17.544401 templated_setup-0.967/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.967/README.md
+-rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 10:16:17.545634 templated_setup-0.967/setup.cfg
+-rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.967/setup.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 10:16:17.539712 templated_setup-0.967/templated_setup/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    18192 2024-05-02 10:15:11.000000 templated_setup-0.967/templated_setup/__init__.py
+-rw-r--r--   0 joel-watson   (501) staff       (20)       21 2024-05-02 10:16:17.000000 templated_setup-0.967/templated_setup/_hardcoded_version.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 10:16:17.543502 templated_setup-0.967/templated_setup.egg-info/
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2477 2024-05-02 10:16:17.000000 templated_setup-0.967/templated_setup.egg-info/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)      248 2024-05-02 10:16:17.000000 templated_setup-0.967/templated_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 10:16:17.000000 templated_setup-0.967/templated_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 10:16:17.000000 templated_setup-0.967/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.965/LICENCE` & `templated_setup-0.967/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.965/PKG-INFO` & `templated_setup-0.967/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.965
+Version: 0.967
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
 
-## V0.965 released on 2nd/5/2024
-god please kill me. ;(
+## V0.967 released on 2nd/5/2024
+Almost decent working condition.
```

### Comparing `templated_setup-0.965/README.md` & `templated_setup-0.967/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.965/templated_setup/__init__.py` & `templated_setup-0.967/templated_setup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 		f"[ END ] {_Setup_Helper.__reload_cached_data}"
 
 
 
 	@classmethod
 	def __load_date(cls, override=False) -> "None":
 		
-		assert cls._json_data
+		assert cls._json_data is not None
 		assert not cls._is_using_pip
 
 		if not override:
 			if "date" in cls._json_data:
 				cls._date_of_last_modified = cls._json_data["date"]
 			else:
 				while True:
@@ -261,15 +261,15 @@
 
 		f"[ END ] {_Setup_Helper.__load_date}"
 
 
 
 	@classmethod
 	def __inner_load_date(cls) -> "None":
-		assert cls._json_data
+		assert cls._json_data is not None
 		assert not cls._is_using_pip
 		do_want_to_use_current_date = _Setup_Helper.__get_y_n("Would you like to use the current date?")
 		new = None
 		if do_want_to_use_current_date:
 
 			cls._date_of_last_modified = datetime_x_date.today()
 			cls._json_data["date"] = cls._date_of_last_modified.isoformat()
@@ -290,15 +290,15 @@
 			year = int(_Setup_Helper.__get_answer(
 				"What year was it last modified? ",
 				lambda x: (x.isdigit(), "Please enter a number."))
 			)
 
 			try:
 				cls._date_of_last_modified = datetime_x_date(year, month, day)
-				assert cls._json_data
+				assert cls._json_data is not None
 				cls._json_data["date"] = cls._date_of_last_modified.isoformat()
 				new = cls._date_of_last_modified.isoformat()
 			except ValueError:
 				print("] Error: Invalid date. Please try again.")
 		
 		assert isinstance(cls._date_of_last_modified, str)
 		cls._date_of_last_modified = new
@@ -306,15 +306,15 @@
 		f"[ END ] {_Setup_Helper.__inner_load_date}"
 
 
 
 	@classmethod
 	def __load_version_number(cls, override=False) -> "None":
 
-		assert cls._json_data
+		assert cls._json_data is not None
 		assert not cls._is_using_pip
 
 		if not override:
 			if "version_number" in cls._json_data:
 				cls._version_number = cls._json_data["version_number"]
 			else:
 				while True:
@@ -330,15 +330,15 @@
 		f"[ END ] {_Setup_Helper.__load_version_number}"
 
 
 
 	@classmethod
 	def __inner_load_version_number(cls) -> "None":
 
-		assert cls._json_data
+		assert cls._json_data is not None
 		assert not cls._is_using_pip
 
 		cls._version_number = _Setup_Helper.__get_answer(
 			"What is the version number? ",
 			_Version.validate_version_number
 		)
 
@@ -349,15 +349,15 @@
 		f"[ END ] {_Setup_Helper.__inner_load_version_number}"
 
 
 
 	@classmethod
 	def __load_notes(cls, override=False) -> "None":
 
-		assert cls._json_data
+		assert cls._json_data is not None
 		assert not cls._is_using_pip
 
 		if not override:
 			if "notes" in cls._json_data:
 				cls._notes = cls._json_data["notes"]
 			else:
 				while True:
@@ -373,15 +373,15 @@
 		f"[ END ] {_Setup_Helper.__load_notes}"
 
 
 
 	@classmethod
 	def __inner_load_notes(cls) -> "None":
 		
-		assert cls._json_data
+		assert cls._json_data is not None
 		assert not cls._is_using_pip
 
 		cls._notes = _Setup_Helper.__get_answer(
 			"Enter the release notes: ",
 			lambda x: (len(x) > 0, "Notes cannot be empty.")
 		)
 
@@ -392,15 +392,15 @@
 		f"[ END ] {_Setup_Helper.__inner_load_notes}"
 
 
 
 	@classmethod
 	def __load_readme_file_path(cls, override=False) -> "None":
 		
-		assert cls._json_data
+		assert cls._json_data is not None
 		assert not cls._is_using_pip
 
 		if not override:
 			if "readme_file_path" in cls._json_data:
 				cls._readme_file_path = cls._json_data["readme_file_path"]
 			else:
 				while True:
@@ -416,15 +416,15 @@
 		f"[ END ] {_Setup_Helper.__load_readme_file_path}"
 
 
 
 	@classmethod
 	def __inner_load_readme_file_path(cls) -> "None":
 
-		assert cls._json_data
+		assert cls._json_data is not None
 		assert not cls._is_using_pip
 
 		cls._readme_file_path = _Setup_Helper.__get_answer(
 			"Enter the path to the README file: ",
 			lambda x: (os.path.exists(x), "File does not exist.")
 		)
 
@@ -441,14 +441,15 @@
 		if not force and not cls._json_data:
 			try:
 				with open(CACHE_FILE_PATH, "r") as f:
 					cls._json_data = json_x_load(f)
 			except FileNotFoundError:
 				force = True
 			if not cls._json_data:
+				cls._json_data = {}
 				force = True
 		if not force and cls._json_data:
 			cls.__load_cached_data()
 			cls.__load_date()
 			cls.__load_version_number()
 			cls.__load_notes()
 			cls.__load_readme_file_path()
```

### Comparing `templated_setup-0.965/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.967/templated_setup.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.965
+Version: 0.967
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
 
-## V0.965 released on 2nd/5/2024
-god please kill me. ;(
+## V0.967 released on 2nd/5/2024
+Almost decent working condition.
```

