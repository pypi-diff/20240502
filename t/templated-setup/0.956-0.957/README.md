# Comparing `tmp/templated_setup-0.956.tar.gz` & `tmp/templated_setup-0.957.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.956.tar", last modified: Thu May  2 09:09:58 2024, max compression
+gzip compressed data, was "templated_setup-0.957.tar", last modified: Thu May  2 09:16:20 2024, max compression
```

## Comparing `templated_setup-0.956.tar` & `templated_setup-0.957.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:09:58.574413 templated_setup-0.956/
--rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.956/LICENCE
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:09:58.573416 templated_setup-0.956/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.956/README.md
--rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 09:09:58.574569 templated_setup-0.956/setup.cfg
--rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.956/setup.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:09:58.569297 templated_setup-0.956/templated_setup/
--rw-r--r--   0 joel-watson   (501) staff       (20)    16859 2024-05-02 09:08:52.000000 templated_setup-0.956/templated_setup/__init__.py
--rw-r--r--   0 joel-watson   (501) staff       (20)      144 2024-05-02 09:03:39.000000 templated_setup-0.956/templated_setup/_hardcoded.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:09:58.572342 templated_setup-0.956/templated_setup.egg-info/
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:09:58.000000 templated_setup-0.956/templated_setup.egg-info/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)      240 2024-05-02 09:09:58.000000 templated_setup-0.956/templated_setup.egg-info/SOURCES.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 09:09:58.000000 templated_setup-0.956/templated_setup.egg-info/dependency_links.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 09:09:58.000000 templated_setup-0.956/templated_setup.egg-info/top_level.txt
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:16:20.341059 templated_setup-0.957/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.957/LICENCE
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:16:20.339620 templated_setup-0.957/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.957/README.md
+-rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 09:16:20.341266 templated_setup-0.957/setup.cfg
+-rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.957/setup.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:16:20.334075 templated_setup-0.957/templated_setup/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    16973 2024-05-02 09:15:03.000000 templated_setup-0.957/templated_setup/__init__.py
+-rw-r--r--   0 joel-watson   (501) staff       (20)      144 2024-05-02 09:03:39.000000 templated_setup-0.957/templated_setup/_hardcoded.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:16:20.338680 templated_setup-0.957/templated_setup.egg-info/
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:16:19.000000 templated_setup-0.957/templated_setup.egg-info/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)      240 2024-05-02 09:16:20.000000 templated_setup-0.957/templated_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 09:16:19.000000 templated_setup-0.957/templated_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 09:16:19.000000 templated_setup-0.957/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.956/LICENCE` & `templated_setup-0.957/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.956/PKG-INFO` & `templated_setup-0.957/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.956
+Version: 0.957
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
 
-## V0.956 released on 2nd/5/2024
+## V0.957 released on 2nd/5/2024
 god please kill me. ;(
```

### Comparing `templated_setup-0.956/README.md` & `templated_setup-0.957/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.956/templated_setup/__init__.py` & `templated_setup-0.957/templated_setup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
 	def __load_date(cls, override=False) -> "None":
 		
 		assert cls._json_data
 		assert not cls._is_using_pip
 
 		if not override:
 			if "date" in cls._json_data:
-				cls._date_of_last_modified = datetime_x_date.fromisoformat(cls._json_data["date"])
+				cls._date_of_last_modified = cls._json_data["date"]
 			else:
 				while True:
 					new = cls.__inner_load_date()
 					confirmed = _Setup_Helper.__get_y_n(f"Is [{new}] Correct?")
 					if confirmed:
 						break
 
@@ -598,14 +598,18 @@
 
 		cls._name = name
 		cls._author = author
 		cls._description = description
 
 		if not cls._is_using_pip:
 			_Setup_Helper.__load_parameters()
+
+			assert isinstance(cls._date_of_last_modified, str)
+			cls._date_of_last_modified = datetime_x_date.fromisoformat(cls._date_of_last_modified)
+
 			assert isinstance(cls._date_of_last_modified, datetime_x_date)
 			assert isinstance(cls._version_number, str)
 			assert isinstance(cls._notes, str)
 			assert isinstance(cls._readme_file_path, str)
 
 			cls._version = _Version(
 				date=cls._date_of_last_modified,
@@ -632,15 +636,14 @@
 	def _finish_setup(cls, kwargs_for_setup_tools:"dict"):
 
 		assert isinstance(cls._date_of_last_modified, datetime_x_date)
 		assert isinstance(cls._version_number, str)
 		assert isinstance(cls._notes, str)
 		assert isinstance(cls._readme_file_path, str)
 
-
 		long_description = _Setup_Helper.__init_description(cls._readme_file_path)
 		long_description += f"\n## V{cls._version.version_number} released on {cls._version.repr_date()}\n"
 		long_description += cls._notes
 
 		if not cls._is_using_pip:
 			_Setup_Helper.__clear_screen()
 			print(f"Current Directory: [{os.path.abspath(os.getcwd())}].\n\n")
```

### Comparing `templated_setup-0.956/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.957/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.956
+Version: 0.957
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
 
-## V0.956 released on 2nd/5/2024
+## V0.957 released on 2nd/5/2024
 god please kill me. ;(
```

