# Comparing `tmp/templated_setup-0.91.tar.gz` & `tmp/templated_setup-0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.91.tar", last modified: Thu May  2 02:08:10 2024, max compression
+gzip compressed data, was "templated_setup-0.92.tar", last modified: Thu May  2 02:21:24 2024, max compression
```

## Comparing `templated_setup-0.91.tar` & `templated_setup-0.92.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 02:08:10.929757 templated_setup-0.91/
--rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.91/LICENCE
--rw-r--r--   0 joel-watson   (501) staff       (20)     2465 2024-05-02 02:08:10.928798 templated_setup-0.91/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.91/README.md
--rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 02:08:10.929913 templated_setup-0.91/setup.cfg
--rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 01:36:24.000000 templated_setup-0.91/setup.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 02:08:10.924931 templated_setup-0.91/templated_setup/
--rw-r--r--   0 joel-watson   (501) staff       (20)    19386 2024-05-02 02:07:13.000000 templated_setup-0.91/templated_setup/__init__.py
--rw-r--r--   0 joel-watson   (501) staff       (20)      143 2024-05-02 02:07:57.000000 templated_setup-0.91/templated_setup/_hardcoded.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 02:08:10.928107 templated_setup-0.91/templated_setup.egg-info/
--rw-r--r--   0 joel-watson   (501) staff       (20)     2465 2024-05-02 02:08:09.000000 templated_setup-0.91/templated_setup.egg-info/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)      240 2024-05-02 02:08:10.000000 templated_setup-0.91/templated_setup.egg-info/SOURCES.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 02:08:10.000000 templated_setup-0.91/templated_setup.egg-info/dependency_links.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 02:08:10.000000 templated_setup-0.91/templated_setup.egg-info/top_level.txt
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 02:21:24.991720 templated_setup-0.92/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.92/LICENCE
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2465 2024-05-02 02:21:24.990052 templated_setup-0.92/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.92/README.md
+-rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 02:21:24.992028 templated_setup-0.92/setup.cfg
+-rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 02:18:46.000000 templated_setup-0.92/setup.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 02:21:24.948526 templated_setup-0.92/templated_setup/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    20070 2024-05-02 02:20:47.000000 templated_setup-0.92/templated_setup/__init__.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 02:21:24.950940 templated_setup-0.92/templated_setup.egg-info/
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2465 2024-05-02 02:21:24.000000 templated_setup-0.92/templated_setup.egg-info/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)      210 2024-05-02 02:21:24.000000 templated_setup-0.92/templated_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 02:21:24.000000 templated_setup-0.92/templated_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 02:21:24.000000 templated_setup-0.92/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.91/LICENCE` & `templated_setup-0.92/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.91/PKG-INFO` & `templated_setup-0.92/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.91
+Version: 0.92
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
 
-## V0.91 released on 2nd/5/2024
+## V0.92 released on 2nd/5/2024
 god please kill me. ;(
```

### Comparing `templated_setup-0.91/README.md` & `templated_setup-0.92/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.91/templated_setup/__init__.py` & `templated_setup-0.92/templated_setup/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -502,14 +502,18 @@
 					user_wants_to_change_params = False
 					continue
 				callback = options[choice-1][1]
 				callback()
 				continue
 
 			if force:
+				assert cls._date_of_last_modified
+				assert cls._version_number
+				assert cls._notes
+				assert cls._readme_file_path
 				json_data = {}
 				json_data["date"] = cls._date_of_last_modified.isoformat()
 				json_data["version_number"] = cls._version_number
 				json_data["notes"] = cls._notes
 				json_data["readme_file_path"] = cls._readme_file_path
 				with open(CACHE_FILE_PATH, "w") as f:
 					json_x_dump(json_data, f)
@@ -631,14 +635,18 @@
 		assert json_data is not None
 		cls._json_data = json_data
 
 		if cls._is_using_pip:
 			cls._json_data_when_using_pip = json_data
 			return None
 
+		if not json_data:
+			assert cls._json_data is not None
+			j_data = cls._json_data
+
 		cls._date_of_last_modified = datetime_x_date.fromisoformat(j_data.get("date", None))
 		cls._version_number = j_data.get("version_number", None)
 		cls._notes = j_data.get("notes", None)
 		cls._readme_file_path = j_data.get("readme_file_path", None)
 
 		return None
 	
@@ -681,15 +689,26 @@
 		cls._version = _Version(
 			date=cls._date_of_last_modified,
 			version_number=cls._version_number,
 			notes=_Setup_Helper.__parse_notes(cls._notes)
 		)
 		cls._version.validate()
 
-		cls._finish_setup(kwargs_for_setup_tools)
+		prev_hardcoded = None
+		try:
+			with open(os.path.join(os.path.dirname(__file__), "_hardcoded.py"), "r") as f:
+				prev_hardcoded = f.read()
+			if not prev_hardcoded:
+				raise Exception("The `_hardcoded.py` file is empty. Please run the script again.")
+			os.remove(os.path.join(os.path.dirname(__file__), "_hardcoded.py"))
+			cls._finish_setup(kwargs_for_setup_tools)
+		finally:
+			assert prev_hardcoded
+			with open(os.path.join(os.path.dirname(__file__), "_hardcoded.py"), "w") as f:
+				f.write(prev_hardcoded)
 
 		return None
 
 		f"[ END ] {_Setup_Helper.setup}"
 
 
 
@@ -703,14 +722,15 @@
 	def _finish_setup(cls, kwargs_for_setup_tools:"dict"):
 
 		assert isinstance(cls._date_of_last_modified, datetime_x_date)
 		assert isinstance(cls._version_number, str)
 		assert isinstance(cls._notes, str)
 		assert isinstance(cls._readme_file_path, str)
 
+
 		long_description = _Setup_Helper.__init_description(cls._readme_file_path)
 		long_description += f"\n## V{cls._version.version_number} released on {cls._version.repr_date()}\n"
 		long_description += cls._notes
 
 		if not cls._is_using_pip:
 			_Setup_Helper.__clear_screen()
 			print(f"Current Directory: [{os.path.abspath(os.getcwd())}].\n\n")
```

### Comparing `templated_setup-0.91/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.92/templated_setup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.91
+Version: 0.92
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
 
-## V0.91 released on 2nd/5/2024
+## V0.92 released on 2nd/5/2024
 god please kill me. ;(
```

