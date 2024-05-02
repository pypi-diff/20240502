# Comparing `tmp/templated_setup-0.954.tar.gz` & `tmp/templated_setup-0.955.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.954.tar", last modified: Thu May  2 05:08:49 2024, max compression
+gzip compressed data, was "templated_setup-0.955.tar", last modified: Thu May  2 08:40:43 2024, max compression
```

## Comparing `templated_setup-0.954.tar` & `templated_setup-0.955.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 05:08:49.195574 templated_setup-0.954/
--rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.954/LICENCE
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 05:08:49.194954 templated_setup-0.954/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.954/README.md
--rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 05:08:49.195773 templated_setup-0.954/setup.cfg
--rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.954/setup.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 05:08:49.192686 templated_setup-0.954/templated_setup/
--rw-r--r--   0 joel-watson   (501) staff       (20)    19892 2024-05-02 05:07:22.000000 templated_setup-0.954/templated_setup/__init__.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 05:08:49.194454 templated_setup-0.954/templated_setup.egg-info/
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 05:08:49.000000 templated_setup-0.954/templated_setup.egg-info/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)      210 2024-05-02 05:08:49.000000 templated_setup-0.954/templated_setup.egg-info/SOURCES.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 05:08:49.000000 templated_setup-0.954/templated_setup.egg-info/dependency_links.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 05:08:49.000000 templated_setup-0.954/templated_setup.egg-info/top_level.txt
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 08:40:43.622304 templated_setup-0.955/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.955/LICENCE
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 08:40:43.621022 templated_setup-0.955/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.955/README.md
+-rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 08:40:43.622483 templated_setup-0.955/setup.cfg
+-rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.955/setup.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 08:40:43.579068 templated_setup-0.955/templated_setup/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    20222 2024-05-02 08:39:32.000000 templated_setup-0.955/templated_setup/__init__.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 08:40:43.620134 templated_setup-0.955/templated_setup.egg-info/
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 08:40:42.000000 templated_setup-0.955/templated_setup.egg-info/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)      210 2024-05-02 08:40:43.000000 templated_setup-0.955/templated_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 08:40:42.000000 templated_setup-0.955/templated_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 08:40:42.000000 templated_setup-0.955/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.954/LICENCE` & `templated_setup-0.955/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.954/PKG-INFO` & `templated_setup-0.955/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.954
+Version: 0.955
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
 
-## V0.954 released on 2nd/5/2024
+## V0.955 released on 2nd/5/2024
 god please kill me. ;(
```

### Comparing `templated_setup-0.954/README.md` & `templated_setup-0.955/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.954/templated_setup/__init__.py` & `templated_setup-0.955/templated_setup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,15 +245,15 @@
 
 	@classmethod
 	def __load_date(cls, override=False):
 
 		if cls._date_of_last_modified:
 			cls.__reload_cached_data()
 
-		if not override and cls._json_data is not None:
+		if not cls._is_using_pip and not override and cls._json_data is not None:
 			assert cls._json_data
 			if "date" in cls._json_data:
 				cls._date_of_last_modified = datetime_x_date.fromisoformat(cls._json_data["date"])
 			else:
 				while True:
 					new = cls.__inner_load_date()
 					confirmed = _Setup_Helper.__get_y_n(f"Is [{new}] Correct?")
@@ -267,14 +267,17 @@
 
 		f"[ END ] {_Setup_Helper.__load_date}"
 
 
 
 	@classmethod
 	def __inner_load_date(cls) -> "str":
+		if cls._is_using_pip:
+			cls._date_of_last_modified = datetime_x_date.today()
+			return cls._date_of_last_modified.isoformat()
 		do_want_to_use_current_date = _Setup_Helper.__get_y_n("Would you like to use the current date?")
 		new = None
 		if do_want_to_use_current_date:
 
 			cls._date_of_last_modified = datetime_x_date.today()
 			if cls._json_data:
 				cls._json_data["date"] = cls._date_of_last_modified.isoformat()
@@ -317,15 +320,15 @@
 
 	@classmethod
 	def __load_version_number(cls, override=False):
 
 		if cls._version_number:
 			cls.__reload_cached_data()
 
-		if not override:
+		if not cls._is_using_pip and not override:
 			assert cls._json_data
 			if "version_number" in cls._json_data:
 				cls._version_number = cls._json_data["version_number"]
 			else:
 				while True:
 					new = cls.__inner_load_version_number()
 					confirmed = _Setup_Helper.__get_y_n(f"Is [{new}] Correct?")
@@ -338,15 +341,19 @@
 	
 		f"[ END ] {_Setup_Helper.__load_version_number}"
 
 
 
 	@classmethod
 	def __inner_load_version_number(cls) -> "str":
-		
+
+		if cls._is_using_pip:
+			cls._version_number = "0.0"
+			return cls._version_number		
+
 		cls._version_number = _Setup_Helper.__get_answer(
 			"What is the version number? ",
 			_Version.validate_version_number
 		)
 
 		if cls._json_data:
 			cls._json_data["version_number"] = cls._version_number
@@ -361,18 +368,15 @@
 
 
 
 	@classmethod
 	def __load_notes(cls, override=False):
 
 
-		if cls._notes:
-			cls.__reload_cached_data()
-
-		if not override:
+		if not cls._is_using_pip and not override:
 			assert cls._json_data
 			if "notes" in cls._json_data:
 				cls._notes = cls._json_data["notes"]
 			else:
 				while True:
 					new = cls.__inner_load_notes()
 					confirmed = _Setup_Helper.__get_y_n(f"Is [{new}] Correct?")
@@ -386,14 +390,18 @@
 		f"[ END ] {_Setup_Helper.__load_notes}"
 
 
 
 	@classmethod
 	def __inner_load_notes(cls) -> "str":
 		
+		if cls._is_using_pip:
+			cls._notes = "No notes."
+			return cls._notes
+
 		cls._notes = _Setup_Helper.__get_answer(
 			"Enter the release notes: ",
 			lambda x: (len(x) > 0, "Notes cannot be empty.")
 		)
 
 		if cls._json_data:
 			cls._json_data["notes"] = cls._notes
@@ -408,15 +416,16 @@
 
 
 
 	@classmethod
 	def __load_readme_file_path(cls, override=False):
 		
 		if cls._readme_file_path:
-			cls.__reload_cached_data()
+			cls._readme_file_path = "README.md"
+			return
 
 		if not override:
 			assert cls._json_data
 			if "readme_file_path" in cls._json_data:
 				cls._readme_file_path = cls._json_data["readme_file_path"]
 			else:
 				while True:
@@ -452,24 +461,24 @@
 
 		f"[ END ] {_Setup_Helper.__inner_load_readme_file_path}"
 
 
 
 	@classmethod
 	def __load_parameters(cls, force=False):
+		if cls._is_using_pip:
+			json_data = cls._json_data_when_using_pip
+			assert json_data is not None
+			cls._date_of_last_modified = datetime_x_date.fromisoformat(json_data["date"])
+			cls._version_number = json_data["version_number"]
+			cls._notes = json_data["notes"]
+			cls._readme_file_path = json_data["readme_file_path"]
+			return
 		if not force:
 			cls.__inner_reload_cached_data()
-			if cls._is_using_pip:
-				json_data = cls._json_data_when_using_pip
-				assert json_data is not None
-				cls._date_of_last_modified = datetime_x_date.fromisoformat(json_data["date"])
-				cls._version_number = json_data["version_number"]
-				cls._notes = json_data["notes"]
-				cls._readme_file_path = json_data["readme_file_path"]
-				return
 		user_wants_to_change_params = False
 		if force:
 			user_wants_to_change_params = True
 		while True:
 
 			cls.__clear_screen()
 			print(f"\n\n] Current Infos:")
```

### Comparing `templated_setup-0.954/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.955/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.954
+Version: 0.955
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
 
-## V0.954 released on 2nd/5/2024
+## V0.955 released on 2nd/5/2024
 god please kill me. ;(
```

